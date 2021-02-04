- Conor/Attention Blocks
- [[Roam Change Log]]
    - "{{embed: [[Path Based Find or Create]]}}""Will reference the last block in the path"
        - {{embed: ((GYGyxoNgB))}}
        - {{embed: ((DgJZfbndy))}}
- [[Near Term Roadmap]]
    - "{{[[TODO]]}} Improved Quick Capture"
    - "{{[[TODO]]}} CSS for custom display of block-children"
- 
- [[Conor]]
    - [[Log]]
        - 16:15
            - [[Roam Pairing]] with [[Bardia]] on [[CSS]] and [[BEM]] [*](((crk0qALA4)))
                - [[Dropzone]]
                    - {{[[kanban]]}}
                        - Unseen
                            - 
                        - Seen
                - Goals::
                    - {{[[TODO]]}} Introduce some of [[Roam Pairing]] process to folks
                    - {{[[TODO]]}} Go through some of the [[LESS]] documentation - and see how I might use some of the helper stuff like variables to more systematically write class names.
                    - {{[[TODO]]}} Map out some of the BEM things for our class
                - Help Resources::
                    - [[[[Roam]]::[[BEM]]]] 
                - Items to map out
                    - [[[[Roam]]::[[BEM]]]] of Block Controls "16:15 - 16:24 (9 min) "Planning""
                    - [[BEM]] components
                    - Controls "^^B^^"
                        - Expand ""^^B^^" or "__E__""
                            - current::
                                - `block-expand`
                        - Bullet "^^B^^"
                            -  "__E__"
                                - 
                            - Bullet Inner"__E__"
                            - ```javascript
<span class="simple-bullet-outer cursor-pointer" draggable="true"><span class="simple-bullet-inner"></span></span>```
                - Sublog
                    - 16:15 - 16:24 (9 min) "Planning"
                        - setup
                    - 16:25 - 16:27
                    - - 16:30 
                        - figuring out zoom stuff
                    - 16:30 - 17:17
                        - Focus area
                            - "[[[[Roam]]::[[BEM]]]] of Block Controls "16:15 - 16:24 (9 min) "Planning"""
                        - - 16:39
                        - 16:39 - 16:41
                            - "!!Choice #Conor"
                                - {{[[TODO]]}} #[[Choice]] Name of the Block
                                    - Options::
                                        - 
                                        - 
                                    - Decision::
                        - #[[Tangent]] #[[Meta]] (20 min)
                            - 16:53 - 17:03 (10 min)
                                - One of the things I've been playing around with is the idea of tagging each item with whether they are B, E, or M
                                    - Why
                                        - Will totally affect their naming convention
                                    - What's missing?
                                        - Whether the class actually is sensible at all - or whether it is something that might not actually be a sensible container to exist.
                                - My first approach here was to go with block references - since it seems like these B, E, M are really only locally defined
                                    - Even with the new [[Path Based Find or Create]] - this is too slow
                                        - What I really want is to [locally define](((_9LNrhBPv))) the [[Text Expansion Templates]] so that I am able to reference the blocks with ;m ;b ;e and have it put out the relevant item - in this case a block ref
                                            - 
                                - Previous approach had been to use [[Namespaced Pages]] - but that approach - even when using the styling [[BEM/Element]] or [[BEM/E]] feels both wrong and too slow.
                                - [[Takeaways]]
                                    - "What I really want is to [locally define](((_9LNrhBPv))) the [[Text Expansion Templates]] so that I am able to reference the blocks with ;m ;b ;e and have it put out the relevant item - in this case a block ref"
                                - 
                                - 
                            - 17:03 - 17:11 (7 min)
                                - "What I really want is to [locally define](((_9LNrhBPv))) the [[Text Expansion Templates]] so that I am able to reference the blocks with ;m ;b ;e and have it put out the relevant item - in this case a block ref"
                                    - [[Idea]] - the thing that I've been sort of feeling as I play with this just now
                                        - Particular this area {{[[embed]]: ((XhhDjhvAp))}}
                                            - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2F5dMPiKX7Wc.png?alt=media&token=a8b86acc-96e0-4b7c-8626-fb223ee1d012)
                                        - Is that I want to be able to either
                                            - #[[Workflows]]
                                            - Drag the block directly into another block  - to apply it as a tag
                                            - Turn the block into a sort of stamp
                                        - [Map](((nofaIHwGC))) a choice of any of those three across a whole tree of the things I had laid out.
                                        - 
                            - 17:11 - 17:14 (3 min)
                                - [[Copy Paste]] related [[Feature Requests]] Inspired by  "[Map](((nofaIHwGC))) a choice of any of those three across a whole tree of the things I had laid out." - which refs a block on [[Algorithms of Thought]]
                                    - {{[[TODO]]}} I wish when I copied a block - when it included a reference to something on a another page - when I pasted it in - I brought all the content that was neccessary along with it (created the new page)
                                        - [[Footgun]] - really we should be setting things up so that when you copy paste between dbs - you link to the other db
                                            - [[False]] - you still want a local copy of your own - even if it is linked to the other one - and this should at least be a prompt 
                                                - Bring the whole trail of nested items....
                                                - 
                        - 
                    - 17:17 - 17:28 (11 min)
                        - [[Tangent]] on the use of `{{or: }}` in [here](((iuo6WX9bL)))
                            - If  you set the or up 
                                - test {{or: ((4uQ6tDvp_)) | a}}
                                    - a
                        - 
                    - - 17:33
                        - {{embed: ((LCx6s9PjJ))}}
                    - 17:41
                        - [[Mind[[BEM]]ding - getting your head around Bem syntax]]
                            - ```css
.rm-block .rm--heading {
   .rm-block__children {
     .rm-block__bullet {
       margin-right: -12px;
       opacity: 0;
     }
  }
}
```
                            - {{[[TODO]]}} [[Choice]] Are elements ever sub-elements in [[BEM]] - or is it just always single level of hierarchy?
                                - Specific Instance::
                                    - Is it `.rm-block__controls__bullet` 
                                    - ```javascript
.rm-block
	.rm-block__controls
		.rm-caret
      	.rm-bullet
			.rm-bullet__outer
			.rm-bullet__inner
			``` 
                                        - If you for instance had `.rm-bullet--version` or `.rm-bullet--user-icon` `.rm-bullet--read-status`
- [[Bardia]]
    - [[Log]]
        - [[Roam Pairing]] with [[Conor]] [*](((Db0hKx9HP)))
            - [[Dropzone]] {{[[kanban]]}}
                - Unseen
                - Seen
            - What's the most important component you want to BEM first?
            - [[[[Roam]]::[[BEM]]]] of `{{kanban}}`
                - `.kanban` "^^B^^"
                    - `.kanban__column` "__E__"
                        - `.kanban__column__title` "__E__"
                        - `.kanban__card` "__E__"
                    - `kanban--hint` "**M**", actually should be "__E__"
            - [[[[Roam]]::[[BEM]]]] of right sidebar
                - `.right-sidebar` "^^B^^"
                    - `.right-sidebar--animating` "**M**"
                    - 
            - [[Tangent]]
                - I think the criteria of whether or not something is a [[BEM/Block]] vs [[BEM/Element]] is whether or not that thing ever can live in isolation outside of the block
            - [[Tangent]]
                - My spacemacs crashes when I try to delete too many lines of code at once  with the vim command `nd`
            - [[[[Roam]]::[[BEM]]]] of block
                - `.rm-block`  "^^B^^"
                    - `.controls` "^^B^^" [*](((vNC3FqCMT)))
                        - `.controls__expand`"__E__"  [*](((2PEZS2uoa)))
                    - `.rm-block__bullet` "^^B^^" [*](((-TK4kqN0-)))
                        - `.rm-block__bullet__inner` "__E__" [*](((BHd7_4ut4)))
                        - `.rm-block__bullet__outer` "__E__"
                        - `controls__bullet--version` "**M**"
                    - `.block__ctx-menu`
                        - `block`
            - If the node can live on its own then it is a block 
    - [[Timestamps]]
        - 19:15-
