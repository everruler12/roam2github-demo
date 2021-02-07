- url::
    - https://csswizardry.com/2013/01/mindbemding-getting-your-head-round-bem-syntax/
- content::
    - One of the questions I get asked most frequently is __what do -- and __ mean in your classes?__
    - The answer is thanks to [BEM](http://bem.info/) and [Nicolas Gallagher](http://twitter.com/necolas)…
    - BEM – meaning __block__, __element__, __modifier__ – is a front-end naming methodology thought up by the guys at [Yandex](http://yandex.ru/). It is a smart way of naming your CSS classes to give them more transparency and meaning to other developers. They are far more strict and informative, which makes the BEM naming convention ideal for teams of developers on larger projects that might last a while.
    - It is important to note that I use a naming scheme __based__ on BEM, but [honed by Nicolas Gallagher](http://nicolasgallagher.com/about-html-semantics-front-end-architecture/). The naming techniques covered in this post are not the original BEM ones, but are improved versions that I much prefer. Whatever the actual notation used, they are all based on the same BEM principles.
    - The naming convention follows this pattern:
    - .block {}
.block__element {}
.block--modifier {}
        - .block represents the higher level of an abstraction or component.
        - .block__element represents a descendent of .block that helps form .block as a whole.
        - .block--modifier represents a different state or version of .block.
    - The reason for double rather than single hyphens and underscores is so that your block itself can be hyphen delimited, for example:
    - ```css
.site-search {} /* Block */
.site-search__field {} /* Element */
.site-search--full {} /* Modifier */```
    - The point of BEM is to tell other developers more about what a piece of markup is doing from its name alone. By reading some HTML with some classes in, you can see how – if at all – the chunks are related; something might just be a component, something might be a child, or __element__, of that component, and something might be a variation or __modifier__ of that component. To use an analogy/model, think how the following things and elements are related:
    - ```css
.person {}
.person__hand {}
.person--female {}
.person--female__hand {}
.person__hand--left {}```
    - The top-level block is a ‘person’ which has elements, for example, ‘hand’. A person also has variations, such as female, and that variation in turn has elements. This again, but written in ‘normal’ CSS:
    - ```.person {}
.hand {}
.female {}
.female-hand {}
.left-hand {}```
    - These all make sense, but are somewhat disconnected. Take .female for example; female what? ^^What about .hand; a hand of a clock? A hand in a game of cards? By using BEM we can be more descriptive but also a lot more explicit; we tie concrete links to other elements of our code through naming alone. ^^Powerful stuff.
    - # Featured case study: NHS
    - How I helped the NHS rapidly build a brand new product.
    - [Read case study…](https://csswizardry.com/case-studies/nhs-nhsx-elearning-platform/)
    - Taking the previous .site-search example again, with ‘regular’ naming:
    - <form class="site-search  full">
    <input type="text" class="field">
    <input type="Submit" value ="Search" class="button">
</form>
    - These classes are fairly loose, and don’t tell us much. Even though we can work it out, they’re very inexplicit. With BEM notation we would now have:
    - <form class="site-search  site-search--full">
    <input type="text" class="site-search__field">
    <input type="Submit" value ="Search" class="site-search__button">
</form>
    - We can see that we have a block called .site-search which has an element which lives inside it called .site-search__field. We can also see that there is a variation of the .site-search called .site-search--full.
    - Let’s take another example…
    - If you are familiar with OOCSS then you will no doubt be familiar with [the media object](http://stubbornella.org/content/2010/06/25/the-media-object-saves-hundreds-of-lines-of-code). In BEM form, the media object would now read:
    - .media {}
.media__img {}
.media__img--rev {}
.media__body {}
    - From the way this CSS is written we can already glean that .media__img and .media__body must live inside .media and that .media__img--rev is a slight variation on .media__img. All that information gathered from the names of our CSS selectors alone!
    - Another benefit is the combatting of the following situation. If we take the media object again:
    - <div class="media">
    <img src="logo.png" alt="Foo Corp logo" class="img-rev">
    <div class="body">
        <h3 class="alpha">Welcome to Foo Corp</h3>
        <p class="lede">Foo Corp is the best, seriously!</p>
    </div>
</div>
    - From looking at this, we can’t see how the classes .media and .alpha are related to each other? Are they? What about .body and .lede or .img-rev and .media? From that HTML (unless we’re very familiar with the media object) we have no idea what makes up that component and what else is optional. If we were to rework it with BEM:
    - <div class="media">
    <img src="logo.png" alt="Foo Corp logo" class="media__img  media__img--rev">
    <div class="media__body">
        <h3 class="alpha">Welcome to Foo Corp</h3>
        <p class="lede">Foo Corp is the best, seriously!</p>
    </div>
</div>
    - We can now instantly see that .media is the block, .media__img--rev is an element of .media that has a modifier applied and .media__body is an unmodified element of .media. All through the names of their classes. That is incredibly useful.
    - ## Uuuugly!
        A common argument against BEM is that it’s ugly; I dare say that if you shy away from code based __purely__ on its looks then you’re often missing the point. Unless the code becomes unnecessarily difficult to maintain, or genuinely more difficult to read, then perhaps you __do__ need to think twice before using it, but if it ‘just looks odd’ but has a valid purpose, then it should definitely be fully considered before writing it off.
        I agree that BEM does look weird, but the power it brings __far__ outweighs any negatives to do with its appearance by an order of magnitude…
        BEM may look a little funny – and it might require more typing (most text editors have autocomplete, and gzip will negate any differences in filesize) – but it is so powerful.
    - ## To BEM or not to BEM?
        - I use BEM notation on everything I build now as its usefulness has proved itself over and over. I’d strongly encourage others to consider adopting it as well because it just makes everything a lot tighter and more connected, making code easier to maintain by teams, or even just by yourself a few months down the line.
        - When you are using BEM, though, it is important to remember that you don’t need to use it for everything. Take for example:
            - [[exceptions]] for [[BEM]] [[[[Skill Tree]] [[Templates]]]]
                - .caps { text-transform: uppercase; }
                - This CSS would never fall into any BEM category, it’s merely a standalone rule.
                - Another example of code which isn’t BEM:
                - .site-logo {}
                - Here we have our logo; it could be BEMmed up like so:
                - .header {}
.header__logo {}
                - But that is unnecessary. The trick with BEM is knowing when something falls into a relevant category. "^^**Just because something happens to live inside a block it doesn’t always mean is is actually a BEM element.**^^ #[[important]] #[[BEM/Element]] [->](((Y_LYlGyTw)))" In the case of our site logo it lives in the .header purely coincidentally; it could just as easily be in our sidebar or footer. An element’s scope can start in any context, so you need to make sure you only apply BEM as far as you need to. Another example:
                    - ^^**Just because something happens to live inside a block it doesn’t always mean is is actually a BEM element.**^^ #[[important]] #[[BEM/Element]] [->](((Y_LYlGyTw)))
            - ```html
<div class="content">
    <h1 class="content__headline">Lorem ipsum dolor...</h1>
</div>```
                - Here "```html
<div class="content">
    <h1 class="content__headline">Lorem ipsum dolor...</h1>
</div>```" "we might be able to just call [the second class](((rusAiUog5)))  .headline; "it depends on "if "{{it: content__headline }}" is styled that way because it’s in .content," or whether ""{{it: content__headline }}" just __happens__ to live in .content"." If it is the latter then we do not need BEM."
                    -  If it is the latter then we do not need BEM.
                    - "{{it: content__headline }}" just __happens__ to live in .content
                    - we might be able to just call [the second class](((rusAiUog5)))  .headline; 
                    - if "{{it: content__headline }}" is styled that way because it’s in .content,
                        - {{it: content__headline }}
        - Everything is potentially open to moving into BEM territory, though. Taking our .site-logo example again, imagine that we want to have a festive version of the logo for our Christmassy site design. We could have:
        - .site-logo {}
.site-logo--xmas {}
        - We can quickly build variations of things by using the -- modifier notation.
        - One of the hardest parts of BEM is deciding when to start and stop scope, and when (or not) to use it. It’s a case of ‘you’ll just know when you know’.
    - ## Final word
    - So that’s BEM (or a slight variation thereof); a highly useful, powerful and simple naming convention to make your front-end code easier to read and understand, easier to work with, easier to scale, more robust and explicit and a lot more strict.
    - For all BEM looks a little odd, it as a hugely valuable addition to the front-end developer’s toolbox, no matter the project.
