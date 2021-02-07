- Components::
    - [[BEM/Block]]
        - "Block: The sole root of the component."
    - [[BEM/Element]]
        - "Element: A component part of the Block."
            - is a smaller part of the another entity
            - "Here "```html
<div class="content">
    <h1 class="content__headline">Lorem ipsum dolor...</h1>
</div>```" "we might be able to just call [the second class](((rusAiUog5)))  .headline; "it depends on "if "{{it: content__headline }}" is styled that way because it’s in .content," or whether ""{{it: content__headline }}" just __happens__ to live in .content"." If it is the latter then we do not need BEM.""
            - "^^**Just because something happens to live inside a block it doesn’t always mean is is actually a BEM element.**^^ #[[important]] #[[BEM/Element]] [->](((Y_LYlGyTw)))"
    - [[BEM/Modifier]]
        - "Modifier: A variant or extension of the Block."
- Decision Tree::
    - Can this "{{or: class|descriptor|entity}}" live entirely on its own?
        - {{or: class|descriptor|entity}}
    - Example::
        - "```html
<div class="content">
    <h1 class="content__headline">Lorem ipsum dolor...</h1>
</div>```"
            - "if "{{it: content__headline }}" is styled that way because it’s in .content,"
            - 
- A systematic approach to naming your [[CSS]] classes
- [[Skill Tree]]
    - BEM, meaning __Block__, __Element__, __Modifier__,
    - BEM splits components’ classes into three groups:
        - Block: The sole root of the component.
            - `.person { }`
        - Element: A component part of the Block.
            - Elements are delimited with two (2) underscores (__)
            - `.person__head { }`
        - Modifier: A variant or extension of the Block.
            - `.person__head { }`
            - Modifiers are delimited by two (2) hyphens (--).
- Basics
    - Example::
        - ```javascript
.person { }
.person__head { }
.person__head { }```
        - "Elements are delimited with two (2) underscores (__)"), and "Modifiers are delimited by two (2) hyphens (--)."
        - ```css
.room { }

  .room__door { }

.room--kitchen { }


.person { }

  .person__head { }```
- Modifying Elements
    - from https://cssguidelin.es/#bem-like-naming
        - You can have variants of Elements, and these can be denoted in a number of ways depending on how and why they are being modified. Carrying on with our person example, a blue eye might look like this:
            - `.person__eye--blue { }`
                - Here we can see we’re directly modifying the eye Element.
        - Things can get more complex, however. Please excuse the crude analogy, and let’s imagine we have a face Element that is handsome. The person themselves isn’t that handsome, so we modify the face Element directly—a handsome face on a regular person:
            - `.person__face--handsome { }`
                - But what if that person __is__ handsome, and we want to style their face because of that fact? A regular face on a handsome person:
                    - `.person--handsome .person__face { }`
                    - Here is one of a few occasions where we’d use a [descendant selector](((Xqn7Z7QDw))) to modify an Element based on a Modifier on the Block.
                        - If using [[Sass]], we would likely write this like so:
                            - ```css
.person { }

  .person__face {

    .person--handsome & { }

  }

.person--handsome { }```
        - Note that we do not nest a new instance of .person__face {} inside of .person--handsome {}; instead, we make use of Sass’ parent selectors to prepend .person--handsome onto the existing .person__face {} selector. This means that all of our .person__face {}-related rules exist in once place, and aren’t spread throughout the file. This is general good practice when dealing with nested code: keep all of your context (e.g. all .person__face {} code) encapsulated in one location.
- Important ideas
    - If using Sass, we would likely write this like so:
    - .person { }

  .person__face {

    .person--handsome & { }

  }

.person--handsome { }
    - Note that we do not nest a new instance of` .person__face {}` inside of `.person--handsome {}`; instead, we make use of {{or: [[LESS]] | [[Sass]]}}’ parent selectors to prepend .person--handsome onto the existing .person__face {} selector. This means that all of our .person__face {}-related rules exist in once place, and aren’t spread throughout the file. This is general good practice when dealing with nested code: keep all of your context (e.g. all .person__face {} code) encapsulated in one location.
