- Office hours
    - When you copy/paste a block, and a block which references it into a new database, it will create two new blocks -- which makes roam/render pretty easy to use.
        - Example::
            - {{roam/render: ((lzFJr9YCu))}}
                - ```clojure
(defn hello []
  [:button.bp3-button {:on-click #(js/alert "Hey Adam")} "Copy Paste this into your db"])```
        - This also works for templates
            - Sample calculation [[roam/templates]]
                - This will do multiplication
                    - A * B =  {{calc: ((DbOmtw4FP)) * ((Nisyw5VJW)) }}
                    - A is 4
                    - B is 5
            - 
            - This will do multiplication
                - A * B =  {{calc: ((eWcA2fLJO)) * ((as84zCZli)) }}
                - A is 6
                - B is 50
            - 
    - How would you go about doing this https://twitter.com/saisatik/status/1353567549720420353?s=20
        - Possible Answers::
            - If I were trying to get a [[Roam Bounty]] for this, this weekend, without needing anything from the team - here is how I [[Conor]] would approach it.
                - Steps::
                    - {{[[TODO]]}} Decide how you are storing the contextual state -- I would do it with attributes most likely.
                        - I would probably use a dedicated attribute - where Entity is the Command - and the then the blocks in the sidebar are Values
                            - Example::
                                - #Work 
                                    - Loads Sidebar::
                                        - #scheduled
                                        - "{{[[mentions]]: [[Scheduling]]}}"
                                            - {{[[mentions]]: [[Scheduling]]}}
                                        - 
                                        - 
                                - #Personal 
                    - {{[[TODO]]}} write a roam/js function - which creates a click handler for a link or tag of the thing you have that loads a context
                    - {{[[TODO]]}} on-click simulate opening those blocks in the search field, and hitting shift-enter in order to open them in the sidebar.
- [[Log]]
    - 15:18 - 15:41 "Office hours" Q and A
    - 15:41 - 15:44 (3 min) writing up "Office hours"
    - 16:11 - 19:30 (3 hours 20 min)
        - 17:05 - 17:19
            - [[User interviews]] [[Sam Corcos]] -- showing his [[Notion]] [[Workflow]] - [[CEO]]/[[Founder]] - [[Startups]]
                - {{[[video]]: https://www.loom.com/share/13f19596b2f14d4aa2ccc1018cc16d34}}
                    - [[Project]] - [[Long Term]] [[roam/js]] [[Roam Bounties]] -- [[High Priority]] - [[Hunch]]
                        - #branch/email-integration
                            - {{[[TODO]]}} Searching your email for unlinked references
                                - Seems pretty doable 
                                - [[V2]] - Grab the names and email addresses and put it into a real structure.
                                    - Related:: [[branch/aliases]], [[project/user-defined-schemas]] and [[project/Ontologies]]
                                    - 
                    - Takeaway::
                        - Takes him 5- 10 minutes to do prep for a single call. We could absolutely get this down to 45 seconds.
            - 
        - 17:19 - 19:30 (2 hours 10 minutes)
            - [[Twitter Thread]]
                - So @SamCorcos from Levels is currently visiting the Roam Compound, and <shock/horror!> he uses Notion...

Gracious host that I am, I offered MULTIPLE reasons Roam might just not be a good fit for him yet, but he INSISTED on showing me a video of workflow

Whoa boy was I wrong

🧵
                    - Draft Chain::
                        - So @SamCorcos from Levels is currently visiting the Roam compound, and <shock/horror> he is not an active Roam user.

Gracious host that I am, I offered up a number of legitimate reasons that Roam might just not be right for him yet -- but he insisted on showing me a video of Notion workflow.

Whoa boy was I wrong. {{count}}
                            - Edited::
                                - So @SamCorcos from Levels is currently visiting the Roam Compound and <shock/horror>.. he uses Notion

Gracious host that I am, I offered up MULTIPLE reasons that Roam might just not be right for him yet, but he INSISTED on showing me a video of workflow.

Whoa boy was I wrong 🧵{{count}}
                                    - Edited::
                                        - So @SamCorcos from Levels is currently visiting the Roam Compound and <shock/horror>... he uses Notion

Gracious host that I am, I offered MULTIPLE reasons Roam might just not be a good fit for him yet, but he INSISTED on showing me a video of workflow

Whoa boy was I wrong

🧵{{count}}
                                            - Edited::
                                                - "So @SamCorcos from Levels is currently visiting the Roam Compound, and <shock/horror!> he uses Notion...

Gracious host that I am, I offered MULTIPLE reasons Roam might just not be a good fit for him yet, but he INSISTED on showing me a video of workflow

Whoa boy was I wrong

🧵"
                - Here is the video - It's 10 minutes long, and he goes through his routine of preparing for calls the night before they happen.

I tried to stop him there - (Not only do I rarely prep calls, whenever possible I refuse to schedule them in advance)

But I get it now {{count}}
                - More importantly, it gave me at least 3 ideas for how we could make Roam even better for someone with a workflow like Sam's - and at least one of them is probably going to be the focus of one of upcoming RoamGames -- 

(See... I knew I would think of one before tomorrow) {{count}}
                - @ 17:52 
                - So what's the big deal?  

Like so many things - it all goes back to the 1950s, -- and the question of "How much of our thinking time is spent thinking, versus getting in a position to think"

![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fv8%2Fhelp%2Fb9ttX-ocn5?alt=media&token=f248b4b1-7362-4c0d-89c0-b8ea3d462f7f)

https://www.rheingold.com/texts/tft/07.html#Chap07 {{count}}
                    - his observations revealed that about 85% of his "thinking" time was actually spent "[[getting into a position to think]], to make a decision, to learn something I needed to know. Much more time went into finding or obtaining information than into digesting it."
                        - 
                    -  https://twitter.com/Conaw/status/1308673469383544832
                - If you watch this video - it takes Sam about 10 minutes to prep for 2 calls. 

granted, he is taking a bunch of time to explain the process

But either way, this one activity adds up to hours per week

Is that CEO Grade thinking time, or time spent just to get in place to think?
{{count}}
                - But time isn't the only issue - there is something much more risky at play here - the cost of context switching

First - just count how many times he is switching back and forth between his email, Notion, his calendar {{count}}
                - Before I saw the video Sam told me the thing he hated most was context switching.

I figured then that much of Roam's design might bother him -- since I EXPLICITLY designed it to make it easy for me to capture as much value from random tangents as possible.{{count}}
                    - Draft Chain::
                        - Before I saw the video - Sam mentioned that there was one thing above all others he hated - which is context switching.

I claimed this is probably a reason certain parts of Roam's design might bother him -- since I EXPLICITLY designed it to make it easy for me to capture as much value from random tangents as possible.{{count}}'
                            - Edited::
                                - "Before I saw the video Sam told me the thing he hated most was context switching.

I figured then that much of Roam's design might bother him -- since I EXPLICITLY designed it to make it easy for me to capture as much value from random tangents as possible.{{count}}"
                - If you've been following me for a while (or God help you you've had to work with me)- you may have gathered this already... but I'm not really a shining pillar of structure and regularilty

The only working style that has ever worked for me is one where I "Ride the Lightning"  {{count}}
                - When inspiration - and more importantly MOTIVATION strikes - more often than not I'm going to drop whatever I'm doing and follow that thread across as many tangents as it is going to take me. {{count}}


                - Like Dave Chapelle says, when an idea takes over, it's the one driving, sometimes I'm in the passenger seat - but more often I'm in the trunk
{{count}}
                - So so often - I've found that if I don't seize the moment and get an idea flushed out - it escapes me. Or it'll take 3 months dragging before I find myself with enough energy to do something that in THAT moment was the most exciting thing in the world. {{count}}
                - This style of operating has not made my life easier -- as you can imagine, I was not the greatest student - when I was finally diagnosed with ADHD in my teens, doctor told my mother I was one of the most severe cases he had seen. 

"How did he get into college without meds?"{{count}}
                - If I'm being honest - one of the main reasons I was drawn to entrepreneurship was because I figured one of the only ways I'd actually be able to hold down a job was if I was the boss.

{{count}}
                - I've said before - there tend to be two kinds of people who are living in the future -- the performance athletes -- the folks who are in such ruthless competition that they will try anything and everything to get the highest performance possible... and the handicapped {{count}}
                - I know Roam's UX is not for everyone -- if you're the Type A striver who already has a system for everything, and has no struggle following that system on a daily, hourly basis -- the main thing you'll notice about Roam is that it takes more effort to make your workspace pretty. {{count}}
                - For me though, Roam really is the Iron Man suit that let me finally walk fast enough to keep up with the other kids.


                - And one of the most important parts of it - when something clicks 

1.  I won't get stuck looking for something I know I have in order to take the next step

2.  I don't need to worry about where I'm putting this work - because when the time is right I'll find it again.  {{count}}
                    - Draft Chain::
                        - And one of the most important parts of it -- when something clicks, and I see a path through a hard problem I can feel confident about two things 

1.  I won't get stuck looking for something I need to take the next step

2.  I don't need to worry about where I'm putting this work - because when the time is right I'll find it again. {{count}}
                            - Edited::
                                - "And one of the most important parts of it - when something clicks 

1.  I won't get stuck looking for something I know I have in order to take the next step

2.  I don't need to worry about where I'm putting this work - because when the time is right I'll find it again.  {{count}}"
                - Everything else is just a bonus -- little aids designed to make it easier for me to stumble into a space that is already prepared for the thinking I need to do.
                - @ 19:02 
                - Now - to get back to Sam's workflow 

In Roam, much of the info he is tracking in his head, or needing to search his email for you get essentially for free -- and you don't even need to use the fancy features.  Just linked and unlinked references.
{{count}}

                - I would be shocked if we couldn't cut the non-thinking part of that work in half {{count}}
                - But it's not like Sam hasn't heard of Roam, or tried it.

And yet - he hasn't made the switch...

Why not? {{count}}
                - Don't say Mobile App.
                - My guess is it has to do with aesthetics -- if you've got the discipline to follow a system like his manually - AND - it isn't clear how the new tool meets that need better AND you're going to have to poke around github and write css yourself to get it pretty... No big surprised{{count}}
                - And usually - when I see someone who has gotten their life as organized and as tuned up as Sam seems to have his - I say - hey, we're not for you just yet 
 There are 100+ Million people with ADHD, and many more than that who already know the tools out there don't support them. {{count}}
                - But something was different today - (probably because I had just come off a 2+ hour call having my mind blown by what @housang had built with roam/js), and throughout the talk, I just kept noticing all the ways we could cut the effort for this workflow by 90% instead of 50%.
                - Here are the first two - one of them will most likely be the focus of the next round of RoamGames starting tomorrow night.
                - 1. Searching Email for Unlinked References.

I've seen RoamHacker query the dictionary - proprietary databases, and just about everything with an API in his alternate sidebars - Why should we ever be searching email from inside a client for context about an encounter. {{count}}
                - 2. Proper aliases, user defined schema, and semantic entities

More specifically - a proper way of connecting people, institutions, email addresses. 

For inspiration there - I recommend http://steve-yegge.blogspot.com/2008/10/universal-design-pattern.html {{count}}
                - 19:30
                - 
                - 
                - 
                - And sure, his brother is @ccorcos - who I know for much of the past few years was responsible for majority of Notion's codebase...

But Sam isn't going to 
                - 

