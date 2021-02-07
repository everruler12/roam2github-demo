- [[Roam Change Log]]
    - Customize display of Roam Blocks based on the links in them, and the links above them.
        - {{[[video]]: https://www.loom.com/embed/06b03473bcda4728b5bef40929e5012f}}
            - # Horizontal Children
                - Testing css customizations #horizontal
                    - How it works                                     .
                        - Put some code like this in a page called [[roam/css]]
                        - This will have every set of nested children grouped into columns
                    - "```css
.roam-block-container[data-page-links*="horizontal"] 
.rm-block-children {
  display: flex;
  flex-direction: row;
 
}
.roam-block-container[data-page-links*="horizontal"] 
 .rm-block__controls {
  display: none;
 
}```"
                        - `.roam-block-container[data-page-links*="horizontal"] .rm-block-children {
display: flex;
  flex-direction: row;
}`
            - Now let's hide that tag "Hide the tag" #rm-h **click and you'll see** `rm-h`
                - A
                - B
                - C
            - # .rm-grid 
                - Let's try a quick grid #rm-grid "Grid `#rm-grid`"
                    - A
                    - B
                    - C
                    - D
                    - E
                    - F
                    - G
                - We can mix the tags up too #rm-blue-border--children #rm-grid
                    - a
                    - b
                - And let's make a particular item span two columns
                    -  #rm-grid #rm-blue-border--children 
                        - A #rm-col-span2
                        - B
                        - C
                        - D
                        - F #rm-col-span2
                        - E
                - And make another that has two rows - while we're at it
                    -   #rm-grid #rm-blue-border--children 
                        - A #rm-col-span2
                        - B
                        - C
                        - D is a larger block of text which will span 2 rows #rm-row-span2
                        - F #rm-col-span2 #rm-row-span2
                        - A
                        - B 
                        - E #rm-col-span2  #rm-row-span2
                        - C
                        - D
                        - 
                - And as our last trick - let's just make every tag that starts with rm-hidden #rm-hide
                    -   #rm-grid #rm-blue-border--children  "```css
.roam-block-container[data-page-links*="rm-hide"]
span.rm-page-ref[data-tag*="rm"] 
{
  display: none;
}```"
                        - A #rm-col-span2
                        - B
                        - C#rm-row-span2
                        - F #rm-col-span2 "![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2F5UewMaPENW.png?alt=media&token=5f0da069-4d80-442c-9081-207f4c0c8edf)"
                        - D
                        - D is a larger block of text which will span 2 rows #rm-row-span2
                        - E
                        - A
                        - B 
                        - # This is a Bigger Area  #rm-row-span2
                        - C
                        - Another
                        - The last one
    - [[New Features]]
        - [[Expandable Parentheticals]]
            - How it works::
                - If you type `((with text inside - but NOT converted into a block reference))` it will now display like this ((((91CCj9YQc)) that's the ((symbol you see here)) ))
                    - thanks to [[@Juvoni]] for showing us the [[Unicode [[Astrolabe]]]] 
                - Clicking on the astrolabe will expand the parenthetical.
                - Clicking on either parenthesis of the open block will close the Parenthetical
                - 
            - Limitations::
                - (([[Links]] and )) ((other **formatted**)) text will not parse ((((c3NvrBVHc))))
                    - Workaround::
                        - Block References do parse - so you can extract any rich text into a block and then wrap the block ref in a parenthetical
            - 
            - [[Ancestors]] and [[inspiration]]
                - We're tempted to call this [[Telescopic Text]] - but the real version of that seems much more impressive
                    - The Ones Who Crossed The Rubicon:: 
                        - https://twitter.com/azlenelza/status/1331583299957911554?s=20
                        - https://getcoleman.com/
                        - https://www.telescopictext.org/text/KPx0nlXlKTciC
                        - [[Stretch Text]] from [[Ted Nelson]]
                            - https://en.wikipedia.org/wiki/StretchText
