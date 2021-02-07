- 17:17
    - Working on a new [[Onboarding Flow]] to replace [[Welcome to Roam]]
        - structure will be sort of like a slide deck or wizard that new users step through, to introduce them to the core ideas, and then step by step teach them the core features they need
            - content
                - Introduction
                    - Roam Research
                        - A Place for Networked Thought
                    - The Web isn't finished
                    - Today the web looks like this
                        - ## One-way links pointing to pages
                        - ![Web Pages Today Keynote Graph](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2F4C8nj9GkBL?alt=media&token=2846b1f6-8272-4ee4-a84e-247f4779a0f3)
                    - ## And knowledge management tools take a "file cabinet" approach to organizing information
                        - ![Files in Folders Keynote Illustration](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FdgYyXuiqwZ?alt=media&token=add58199-9b74-460c-a671-a5582cbace54)
                    - ## The human mind works more like this
                        - ![Omnigraffle Idea Image](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FBBbdQEzVHF?alt=media&token=b5e2c132-6e24-47a2-8bf7-f7b85a525efe)
                        - A graph of concepts and memories
                        - Collected in overlapping sets
                        - Traversable in any direction
                        - With ability to build new ideas out of old ones
                    - ## Roam is a personal web that works more like your mind
                        - testimonials
                            - pull from [[What People Are Saying]]
                                - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FPfG1NB_mab?alt=media&token=b62c8287-7f95-40c1-b22a-476bbfdb6636)
[source](https://twitter.com/kylemathews/status/1192517571997683712) #[[Kyle Matthews]]
                - Steps
                    - Roam is not about files, it is about managing ideas
                        - [[backlinks]] -- aka [[Bidirectional Links]]
                        - {{[[DONE]]}} add twitter post
- 17:38
    - Building this [[Onboarding Flow]]component out 
        - steps::
            - Each step is going to have 
                1. an event that you need to fire to get to the next step
                2. Demo content in the editable area
                3. Tutorial copy in a view area
                4. Whether the user has completed the step or not
                5. The next step in the tutorial
            - Some of the steps will have
                - Just the Outline component for a single page
                - Multiple components
                    - Filters
                    - The Sidebar
                    - Mentions
- 18:36
    - [[Keyboard Shortcuts]] for switching tabs in chrome
        - https://www.wikihow.com/Switch-Tabs-in-Chrome
        - Control-tab 
            - to go to the tab to the right
        - Control-shift-tab 
            - to go to the tab on the left
        - On [[Mac]]
            - Command-Number
                - Will get you to the numbered tab
        - on [[PC]]
            - Control-Number
                - "Will get you to the numbered tab"
- 18:44
    - "Building this [[Onboarding Flow]]component out "
        - First step to build
            - A screen that just has "Tutorial copy in a view area", "The next step in the tutorial"and "Whether the user has completed the step or not"
        - First real step to build
            - Step 1
                - title::  What not Where
                - tutorial content:: 
                    - Roam is about organizing ideas
                    - Not files
                    - When you want to add something to your grocery list, you do not need to find your grocery list page
                    - Just link to the page, from anywhere
                        - Indent under the link
                        - And add the items there
                - Example::
                    - [[December 9th, 2019]]
                        - Think I'd like to bake an apple pie tonight
                            - [[Grocery List]]
                                - Half dozen apples
                - User Action::
                    - Visit the grocery list page by clicking the link, to view the collected references
                - Next Step:: Step 2
                    - step:: "Step 2" 
                    - label:: Now You try
            - Step 2
                - title:: Create a link
                - tutorial content::
                    - There are multiple ways to create a link
                    - Let's try all three
                        - First, highlight a word or phrase in this list and then hit [ twice
                            - It will wrap the text in [[ and create a link
                - Example::
                    - Conversation with Joshua Brown and Richard Meadows about Roam Research and Knowledge Management
                        - [[Quotes]]
                - User Action::
                    - Part 1
                    - 
        - table
            - {{attr-table: [[title]]}}
- 19:05
    - Thinking that the tutorial might work really well with a use case involving [[Kindle Highlights]]
        - steps here would be 
            - Get your highlights
                - would be great to get them directly from readwise.io
            - Create a list of things you're thinking about 
- 22:24
- [[vgr]][[Tweet]][[@RoamResearch]] [[Tiago Debate]]
    - source:: https://twitter.com/vgr/status/1202387496832618496
    - Alright one week in, I've settled into some steady habits using roam, so there's a habit attractor here. Progress has slowed to more day-to-day but it still feels like winning the war on entropy as opposed to losing it in scrivener, email, or twitter.


    - Gonna start documenting subtle features here. First up: Roam is probably the most efficient prosthetic memory I’ve used, as in, creating efficient recall of thoughts I’ve already thunk and written up. A killer feature when you’ve written as much as I have (good or bad).



    - On a scale of 1 to 10, ranking media I’ve used

Paper: 1 (no recall aids unless you create ToCs or indices yourself)

Email newsletters: 2 (weak searchability, weak theme/thread continuity, weak gestalt, though substack is better than mailchimp)

Twitter: 4 (strong searchability, strong threadability, weak gestalt)

Wiki: 5 (strong searchability, medium threadability, strong gestalt)

Blog: 6 (strong searchability, strong threadability, strong gestalt)

Roam: 8 (all of the above plus low friction update/create/rename)


    - The thing is, recall is a virtuous cycle. The better a medium supports recall, the easier it is to attach new information in the right places. Which makes recall even easier. And the easier it is to add content, the faster this process snowballs. So a [[compound interest]] effect.

    - Knowledge generally depreciates, and a holy grail of knowledge modeling and capture for a long time has been to reverse the default negative interest rate it accrues and turn it positive. There was a “[[knowledge banking]]” project at Xerox back in the day that aimed at this for eg.


    - In the past most such efforts have failed because they relied on automation to try and keep entropy at bay, which sort of works weakly with relative legible and structured information. But for more squishy information, the only thing that works is a “[[many eyeballs]]” process.


    - Anytime I’ve seen a positive-interest-rate knowledge repo, it’s because many people were resurfacing bits and pieces at random and making point improvements. So the only known solution to date for positive interest rate has been to collectivize and socialize the prosthetic memory #[[many eyeballs]]

    - So a good measure of the technical sophistication of a medium is to measure the number of people (eyeballs) and money (how much they’re paid) required to sustain a positive interest rate. I think Roam reduces both to the limit: 1 person and self-funded hobby time. #[[many eyeballs]]

    - Compare for instance Wikipedia (~100s-1000s unpaid) or Stanford Encyclopedia or Wolfram Mathworld (single digits -100s, but paid, directly it indirectly).

This is probably because Roam allows one mind to effectively act as many ([[Fox]] > [[Hedgehog]])

    - In practice, I’m finding now that when I have a new nugget to add, from whatever headspace I’m in (working, at the gym, random thought during in a meeting, half-asleep thought in bed), I can always make a quick judgment  of approximately where a thought belongs, and put it there. #[[What Not Where]]

    - By contrast in weaker media, I have to be in high energy, direct focus headspace, having warmed up around 30 minutes to get situation awareness around the whole project. Only then can I reliably lower entropy and turn interest rate positive. Roam lowers threshold to 10% of that.

    - This btw is the maker time/manager time problem pg wrote about. Making needs 4 hour chunks because anything less tends to increase entropy rather than decrease it in any non-trivial knowledge work project. So anything that lowers that lower limit is a big win. #[[Maker Schedule]]
        - see also "Breaking our work into smaller chunks directly creates the conditions for flow. Smaller packets dramatically impact not just the quantity and speed of work we can produce, and not just its quality, but the actual experienceof producing it. Work becomes more motivating, more meaningful, easier, more impactful, and more engaging. #[[Maker Schedule]]"
    - My suspicion is, a good KPI for a knowledge tool is minimum threshold of time required to make a negentropic update to it, with every halving of the threshold increasing its capacity to hold positive-interest-rate knowledge repos by an order of magnitude.
Venkatesh Rao
@vgr

    - So a tool with a 2h minimum can sustain a 10x bigger positive-rate knowledge base with the same budget of people/money than a 4h minimum. I suspect for Roam, a very suitable project may get it down to minutes, and for a typical project, maybe 30min.

Something like that.
10:44 AM · Dec 8, 2019·Twitter for iPad
16
 Likes
