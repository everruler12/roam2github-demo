- [[Take Home Project]]  [[Backend Role]] [[parser]]
    - Context::
        - https://twitter.com/Conaw/status/1333174002550927360?s=20
    - Folks have asked us for a backend problem - comparable to the screen we put up for [[UI Engineer]]
        - We don't have a first filter problem - so we'll just give you one that is useful for us - and since it is useful - if you meet all these requirements all the way -- we'll give you an immediate bounty of $5,000 - and you'll immediately have passed to the final round of interviews where you meet the whole team.
    - This is not `strictly` backend - it's data transformation - but our team is still mostly front-end engineers, so it's a bit tougher for us to come up with a proper backend problem.
    - Related - if you give us a better problem that we go with instead - and that problem is answered within 1 month -- we'll give you $10,000 -- that's ongoing, for all our roles.
    - description::
        - We try to keep some plaintext representation of all the data folks store in Roam - so that folks can own their data in an actionable real way - take it with them if they leave - or (less risk now that we're profitable and funded) have security if Roam ever disappears.
        - There are some bugs in our parser - it doesn't handle certain kinds of nesting - and it is a bit of a pain to extend -- also - it is painful whenever we want to make up more specific syntax - like for queries.
        - We've been meaning to re-write it.  
        - If you show you can do a better job that we would - we want to talk to you.
    - Scope::
        - 5 - 20 hrs
    - Criteria::
    - {{[[TODO]]}} The parser can parse all of Roam's major syntax at least `[[link]]` `((ref))``{{roam-render}}` `$$latex$$` `[alias](target)` `^^highlight^^` `**bold**` `__italic__`
        - {{[[TODO]]}} The parser is recursive - it can handle [[Nested [[Links]]]] and ^^**bold highlights**^^ and `[html roam]([[Aliases]])`all the ones we haven't done yet as well
        - Specifically ```javascript

Aliases inside aliases
>   
  [![img](image-as-alias.com)](www.roamreasearch.com)

{{{{curly braces}} in{{side}} of {{curly braces}}}}


```
        - {{[[TODO]]}} Return a Tree - with the result of the parse.
        - {{[[TODO]]}} Provide an abstraction for Replacing each item in the tree with something else (like an html component, or a new string value)
            - One aspect of a winning solution might be the equivalent of update-in for a parsed section of the string.
                - Similar to how we might update in a map with swap!
                - aka - you give us the parsed value in an atom - if we reset that atom, it should change the string at the location of the parse.
        - {{[[TODO]]}} Your solution is fast for most cases - it can parse - and replace a string with a hiccup component in - for example 1000strings in under 500ms
            - More points for faster
                - As long as you make it through 95% of them in under 500ms, and push the others off to finish in under 1s
        - {{[[TODO]]}} Other ones to thing about
            - ```javascript
a very winning solution could parse arbitrary code - with an easy abstraction for extending it.
example - using insect.js in calculations - and replacing variables with their definitions.

or taking something like

user wants to find the time between to pieces of text

you write a parser that looks for a pattern like this - and can then replace it.

<%%:%% - %%:%%>
13:41 - 14:03  and then replace the whole thing with tthe result of adding them together - or add the string (time % hours) after


{:inc 1} {:do-something This | That} 
{∆: {:style :snooze, :delay 1day, :every 2hours, :rule (if (= 2 2) (inc :delay) (dec :delay))} }```
            - 
        - 
        - 
