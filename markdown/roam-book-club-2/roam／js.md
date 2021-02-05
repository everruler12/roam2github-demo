- see also: [[roam/css]]
    - (last updated 10:15 AM PST Wednesday [[October 28th, 2020]] by [[Matt Brockwell/MJB]])
- (javascript mods to this database are indented below, to allow "view as numbered list")
    1. The below is David Vargas' JS that allows for the filtering and sorting of linked references. It is here primarily to allow shared users to view and filter group # chat  but also will help, e.g., viewing our directory
        - {{[[roam/js]]}}
            - ```javascript
var old = document.getElementById("sort-references");
if (old) {
  old.remove();
}

var s = document.createElement("script");
s.src = "https://roamjs.com/sort-references.js";
s.id = "sort-references";
s.async = false;
s.type = "text/javascript";
document.getElementsByTagName("head")[0].appendChild(s);```
    2. the below is [[Charlie Mead]]'s work [[plugins/(rand)]] - it will allow users to "pull" random sub-blocks to enhance serendipitous discovery
        - {{roam/js}}
            - ```javascript
const COMMAND = /\(rand\s*\d*\)/;
const ENTER = 'Enter'

const getParentBlock = (childUid) => {
  return window.roamAlphaAPI.q(
    `[:find (pull ?parent [:block/uid :block/string]) \
             :where \
             [?block :block/uid "${childUid}"] \
             [?parent :block/children ?block]]`
  )[0][0]
}

const getBlockUids = (title, n) => {
  return window.roamAlphaAPI.q(
    `[:find (rand ${n} ?uid) :where [?e :node/title "${title}"] [?e :block/children ?x] [?x :block/uid ?uid]]`
  )[0][0]
};

const makeHandler = (str) => (evt) => {
  const match = str.match(/\d+/)
  const n = match ? Number(match[0]) : 1
  
  if (evt.key === ENTER) {
    const uid = evt.target.id.match(/.{9}$/)[0]
    const parentBlock = getParentBlock(uid)
	const title = parentBlock.string.replaceAll('[[', '').replaceAll(']]', '').trim()
    const values = getBlockUids(title, n);
    evt.target.value = values.map(uid => `((${uid}))`).join("\n")
  }
};

const applyListener = () =>
  document.querySelectorAll("textarea").forEach((el) => {
    if (el.value.match(COMMAND)) {
      el.onkeydown = makeHandler(el.value)
    }
  });

const observer = new MutationObserver(applyListener);

observer.observe(document.body, { subtree: true, childList: true });```
    3. EXPERIMENT - suspended for now due to bugs - the below is [[Cato Minor]]'s "roamext" - if you turn on this javascript it will enable some block-level formatting.
        - [[Cato Minor]]'s [[Roamext]] lives here:
            - {{[[roam/js]]}}
                - ```javascript
		

;(()=>{
  
  if( typeof window.catominor_tags != 'undefined') return;

  window.catominor_tags = {};

  const scanTags = () => {
    document.querySelectorAll('[data-tag]').forEach( (element)=>{
      console.log("start");
      let divBlockTagAttributeArray;
      let divBlock = element.parentElement.parentElement;
      const tagAttribute = " " + element.getAttribute('data-tag') + " ";
      
      
      

      
      let divBlockTagAttribute = divBlock.getAttribute("data-tags");
      
      if (divBlockTagAttribute ==  null){
        divBlockTagAttributeArray = [];
      } else {
        
        divBlockTagAttributeArray = divBlockTagAttribute.split(","); 
      }
    
      let index;
	 
      if(element) {
        console.log(tagAttribute);
        let index = divBlockTagAttributeArray.indexOf(tagAttribute);
        if (index == -1) {
       			divBlockTagAttributeArray.push(tagAttribute);
   		 }
     
      } else {
         let index = divBlockTagAttributeArray.indexOf(tagAttribute);
		 if (index > -1) {
       			divBlockTagAttributeArray.splice(index, 1);
   		 }
         
        
        
      }
      console.log(divBlockTagAttributeArray);
      divBlock.dataset.tags = divBlockTagAttributeArray.join();
      divBlock.parentNode.parentNode.parentNode.dataset.tagsUp = " " + divBlockTagAttributeArray.join() + " ";
     // divBlock.parentNode.parentNode.parentNode.childNodes[0].dataset.tagsDown = divBlockTagAttributeArray.join();


      console.log(divBlock.dataset.tags);
  
    })
  }

  scanTags()
  var observerTags = new MutationObserver(scanTags);
  observerTags.observe(document.querySelector('#app'), {
    childList: true,
    subtree: true
  })

})();```
            - here are some #HOW-TO instructions for [[Roamext]]
                - check out this CSS:
                    - ```css

[data-tags~="redborder"] {
  border: 1px solid red;
}

[data-tags-up~="orangeborder"] {
  border: 1px solid orange;
}


[data-tags-up~="blueborder"] > div:nth-child(2) {
border: 1px solid blue;
}


```
                - note that  the datatags commands break down into three "kinds" to handle the classes of block only, block with children, and only-children.
                - #blueborder
