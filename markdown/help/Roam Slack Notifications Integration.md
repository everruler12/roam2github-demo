- Video demonstration:
    - https://www.loom.com/share/f82dec5ff87a4425a4b17624b9e6dfb1
- Steps:
    - Copy and paste the below block into your graph
    - Launch slack in your browser
    - Create and navigate to the channel you want the notifications to be sent to
    - Get the channel ID from the URL (it is the last set of alphanumeric characters)
    - Paste it in `notificationChannel` in the roam/js script
    - Go to https://api.slack.com/start/ while signed in to your workplace
        - Create a Slack app
        - Add it to your workplace
        - Add the following OAuth permissions:
            - channel:read
            - chat:write
            - users:read
            - users:read.email
        - Install the app in the workplace
        - Copy and paste the user oauth access token in `oauthToken` in the roam/js script
        - Add the list of tags you want to use to notify a user and the user's corresponding Slack email in `tagToEmail`
        - Press "Yes, I know what I'm doing"
- {{[[roam/js]]}}
    - ```javascript
// Slack Channel ID 
var notificationChannel = "";
// Token for a Slack App.
var oauthToken = "";
// A map of the notification tag to the email of the user you want to notify
// Email must be the one used in the Slack that contains the channel.
var tagToEmail = {
	// "#[[!bardia]]": "bardia@roamresearch.com"
}

function jsonEncode(baseUrl, json) {
  const url = new URL(baseUrl);
  Object.entries(json).map(([k, v]) => url.searchParams.set(k, v))
  return url.href;
}

async function callSlackAPI(url, data) {
  // Can only submit GET requests to the Slack API via web since they have CORS
  // setup to deny Authentication and Content-Type headers.
  const response = await fetch(jsonEncode(url, { token: oauthToken, ...data }));
  return response.json();
}

async function getUserId(email) {
  // Needs users:read.email permissions.
  const lookupByEmailURL = "https://slack.com/api/users.lookupByEmail";
  const response = await callSlackAPI(lookupByEmailURL, { email });
  return response.ok ? response.user.id : false;
}

async function postNotification(msg) {
  // Needs chat:write permissions.
  const postMessageURL = "https://slack.com/api/chat.postMessage";
  const response = await callSlackAPI(postMessageURL, {
    channel: notificationChannel,
    unfurl_links: false,
    link_names: true,
    text: msg
  });
  return response.ok;
}

async function notifyUserOfLink(email, link, msg) {
  const uid = await getUserId(email);
  if (!uid) {
    return false;
  }
  return await postNotification(`Ping <@${uid}> at ${link}\n${msg}`);
}

function blockLink(blockId) {
  const graph = document.location.href.match(/^.*?\/app\/([^\/]+)\/?/)[1];
  return `https://roamresearch.com/#/app/${graph}/page/${blockId}`;
}

function handleTag(tag, blockId, blockStr) {
  const email = tagToEmail[tag];
  if (email) {
    // console.log("sending notification");
    return notifyUserOfLink(email, blockLink(blockId), blockStr);
  }
}

function newTags(before, after) {
  const tagRegExp = /#(?:\[\[)?([^\s])*(?:\]\])?/g;
  const tagsBefore = before.match(tagRegExp) || [];
  const tagsAfter = after.match(tagRegExp) || [];
  return tagsAfter.filter(t => !tagsBefore.includes(t));
}

function watchBlocksForNewTags() {
  let lastBlockId = null;
  let lastBlockStr = null;
  const callback = function (mutationsList, _) {
    // Events aren't necessarily ordered.
    // First check all the blocks left from and handle new tags.
    for (var mutation of mutationsList) {
      if (mutation.type === 'childList' && mutation.removedNodes.length && mutation.removedNodes[0].childElementCount && mutation.removedNodes[0].children[0].classList.contains('rm-block-input')) {
        const blockId = mutation.target.children[1].id.match(/.{9}$/)[0];
        const str = mutation.removedNodes[0].children[0].textContent;
        // console.log("exit block", blockId, str)
        if (lastBlockId == blockId) {
          const tags = newTags(lastBlockStr, str);
          tags.forEach(t => handleTag(t, blockId, str));
        }
      }
    }
    // Then check what the new block is, if any.
    for (var mutation of mutationsList) {
      // Enter existing block.
      if (mutation.type === 'childList' && mutation.addedNodes.length && mutation.addedNodes[0].childElementCount && mutation.addedNodes[0].children[0].classList.contains('rm-block-input')) {
        const blockId = mutation.target.children[1].children[0].id.match(/.{9}$/)[0];
        const str = mutation.addedNodes[0].children[0].textContent;
        lastBlockId = blockId;
        lastBlockStr = str;
      }

      // Enter new block.
      if (mutation.type === 'childList' && mutation.addedNodes.length && mutation.addedNodes[0].childElementCount &&
        mutation.addedNodes[0].children[0] &&
        mutation.addedNodes[0].children[0].children[0] &&
        mutation.addedNodes[0].children[0].children[0].children[1] &&
        mutation.addedNodes[0].children[0].children[0].children[1].children[0] &&
        mutation.addedNodes[0].children[0].children[0].children[1].children[0].classList.contains('rm-block-input')
      ) {
        const el = mutation.addedNodes[0].children[0].children[0].children[1].children[0];
        const blockId = el.id.match(/.{9}$/)[0];
        const str = el.textContent;
        lastBlockId = blockId;
        lastBlockStr = str;
        // console.log("enter new block", blockId, str)
      }
    }
  };
  // Create an observer instance linked to the callback function
  const observer = new MutationObserver(callback);
  observer.observe(document.body, { childList: true, subtree: true });
}

watchBlocksForNewTags();```
