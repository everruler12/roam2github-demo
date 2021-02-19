- 06:20 - 06:53 (33 minutes)
    - https://twitter.com/Conaw/status/1362758157580136450?s=20
    - - 06:38
        - Quick example of custom block level tags using [[roam/css]]
            - `[[.Falsified]]`
                - "```css
.Falsified {
text-decoration: line-through;
}```"
                - {{[[DONE]]}} Example of something I thought about doing but didn't #.Falsified
                    - Details about this that don't matter, because original assumption is wrong
                        - Query for it
                            - {{[[query]]: {and: [[DONE]] [[.Falsified]]}}}
            - Let's say I wanted to have some ^^__grey text in here__^^ #.grey-hl  
                - "```css
.grey-hl .rm-highlight {
  background-color: transparent;
  color: gray;
}
```"
            - And ^^this^^ is big #.big
                - "```css
.big .rm-highlight {
  background-color: transparent;
  font-size: 2em;
}```"
                - 
            - Tutorial Videos::
                - {{[[video]]: https://www.loom.com/share/f603f87915704a548d00405a5b5e005c}}
    - - 06:53
        - More Thorough Example [[roam/css]]
            - Let's say for  example that I want to have a few nested items listed horizontally 
                - specifically::
                    - I want to think about #.group
                        - A #.group
                            - B
                        - C
                    - as being a group
