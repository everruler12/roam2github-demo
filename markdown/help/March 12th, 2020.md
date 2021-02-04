- Literally found out how to hack styles in Roam super easily -- and get [[Dark Mode]]
    - Just copy paste these blocks - if you keep them open in the sidebar somewhere -they will give you darkmode - changing them is literally as simple as opening and closing the bullet
- Click the arrow next to this bullet to toggle: 
    - #Theme Dark -- via [[Malcolm Ocean]] #[[Dark Mode]]
        - #[[Theme]] Red Dark
            - :hiccup [:style "

.roam-body .roam-app,
.roam-body .roam-app h1,
.bp3-popover .bp3-popover-content,
.bp3-menu {
    color: #e20;
}

.roam-body .roam-app .roam-sidebar-container {
    background-color: #120200;
  
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
        background-color: #120200;
    color: #a20;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover {
    background-color: #320500;
    color: #f40;
}

.bp3-input::placeholder,
.bp3-input-group > .bp3-icon {
    color: #940;
}
.bp3-omnibar {
    background-color: #420;
}
}

"]
        - :hiccup [:style "
body {
    background: black;
}

.roam-topbar {
    background-color: black;
}

.bp3-input,
.bp3-input[readonly]{
    background: black;
    box-shadow: inset 0 0 0 1px rgba(223, 234, 245, 0.15);
}

.roam-body .roam-app,
.roam-body .roam-app h1 {
    color: #c0c6cc;
}

.bp3-popover .bp3-popover-arrow-fill {
    fill: black;
}
.bp3-popover .bp3-popover-content,
.bp3-menu {
    background: black;
    color: #c0c6cc;
    box-shadow: 0 0 0 1px rgba(223, 234, 245, 0.1),
                0 2px 4px rgba(223, 234, 245, 0.2)/*,
                /*0 8px 24px rgba(16, 22, 26, 0.2)*/;
}

.roam-body .roam-app .roam-sidebar-container {
    background-color: #0c1013;
}

#roam-sidebar-logo {
    opacity: 0.4;
}
#roam-sidebar-logo:hover {
    opacity: 0.7;
}

.roam-article > div:last-child div:not(.bp3-icon) {
    background: #111 !important;
}

.roam-article > div:last-child a {
    color: #cc0 !important;
}

.bp3-omnibar {
    background-color: #234;
}
}



"]
        - **Now Red is gone!**
- Use Command-Shift-O to open in the sidebar
- #[[Dark Mode]] #Theme from sjsanc
https://github.com/sjsanc/roam_darktheme
    - Main #Theme
        - :hiccup [:style "  
/*
### ROAM CUSTOM THEME ###
> Based on the Ayu palette from Rust's mdBook
> Edits by Ancestor
> v1.0
*/

/* Import new fonts */
@import url('https://fonts.googleapis.com/css?family=Source+Code+Pro:300,400,500&display=swap');
@import url('https://fonts.googleapis.com/css?family=Open+Sans:300,400,600,700&display=swap');

/* ## ARTICLE STYLING (Article size, margins etc) ## */
.rm-block-text {
  max-width: 1100px;
}
.roam-center div:first-child {
    padding-right: calc(10% - 284px) !important;
    padding-left: calc(34% - 516px) !important;
}
.roam-article {
    width: 1100px;
}
.roam-block-container {
    max-width: 1100px;
}

/* ## COLOURS ##*/
body {
    background-color: #0F1419;
    font-family: 'Open Sans';
}

.roam-app h1 { /* styles page titling */
    color: #C5C5C5 !important;
    font-family: 'Open Sans';
    font-weight: bold;
}

.roam-app { /* primary text colour */
    color: #C5C5C5 !important;
}

.roam-topbar {
    background-color: #182026;
}

.rm-page-ref-tag { /* hashtags */
    color: #69e3ff !important;
    background-color: #263139;
    border-radius: 3px;
    padding: 2px 3px 2px 3px;
}
.rm-page-ref-tag:hover {
    background-color: #353f46;
    text-decoration: none;
}

.block-highlight-blue { /* the bright blue highlight color */
    background-color: #1c2e3e;
}

.block-border-left { /* the tree graphics */
    border-left: 2px solid #343d48;
}

.rm-block-input { /* the currently selected block */
    background-color: #273540;
    border-radius: 3px;
    padding-left: 3px;
}

.rm-reference-item { /* the reference boxes at the bottom */
    background-color: #182026;
}

code { /* the single backtick code snippets */
    background-color: #242F38 !important;
    border-radius: 3px !important;
    color: #fded74;
    border: 0px solid #13191e;
    padding: 3px 4px 3px 4px;
    font-weight: bold;
}

strong { /* bold text */
    font-size: 1.15em;
    color: #c5c5c5;
}
.roam-highlight { /* highlighting */
    background-color: #FDD755;
    color: #0F1419;
    border-radius: 2px;
    padding: 2px 3px 2px 3px;
}
.roam-bullet-closed { /* expandable bullets */
    background-color: #b5f7ff;
}

.rm-pages-row { /* styles colour on the all pages */
    background-color: #182026;
}
.rm-pages-row:first-of-type { /* styles colour of all pages table header */
    background-color: #182026 !important;
}
.rm-pages-row:hover {
    background-color: #273540;
}
.bp3-button.bp3-minimal.bp3-intent-success { /* new page button*/
    color: #5c7080;
}
.bp3-button.bp3-minimal.bp3-intent-success:hover { /* new page button*/
    background: rgba(167,182,194,0.3);;
    color: #fff;
}

#right-sidebar {
    background-color: #2f3e4a !important;
}


/* ### */
.flex-v-box { /* can't remember what this did lol */
    margin-left: 5px !important;
}
.bp3-elevation-3 {
    color: #262626;
}"]
    - #Theme [[Codemirror]] #[[Dark Mode]]
        - :hiccup [:style "

@import url('https://fonts.googleapis.com/css?family=Source+Code+Pro:300,400,500&display=swap');

.CodeMirror{
    font-family:'Source Code Pro' !important;
    height:300px;
    color:white;
    direction:ltr;
    background: #182026 !important;
    border-radius: 5px;
}
.CodeMirror-lines{
    padding:4px 0
}
.CodeMirror pre{
    padding:0 4px;
    margin-left: 5px;
}
.CodeMirror-scrollbar-filler,.CodeMirror-gutter-filler{
    background-color:white
}
.CodeMirror-gutters{
    border-right:0px solid #ddd;
    background-color:#242F38;
    white-space:nowrap;
    width: 30px;
}
.CodeMirror-linenumber{
    padding:0 3px 0 5px;
    min-width:20px;
    text-align:right;
    color:#999;
    white-space:nowrap;
    font-family:'Source Code Pro';
}
.CodeMirror-guttermarker{
    color:black
}
.CodeMirror-guttermarker-subtle{
    color:#999
}
.CodeMirror-cursor{
    border-left:2px solid #394D6C;
    border-right:0;
    margin-left: 0px;
    width:0
}
.CodeMirror div.CodeMirror-secondarycursor{
    border-left:1px solid silver
}
.cm-fat-cursor .CodeMirror-cursor{
    width:auto;
    border:0 !important;
    background:#7e7
}
.cm-fat-cursor div.CodeMirror-cursors{
    z-index:1
}
.cm-fat-cursor-mark{
    background-color:rgba(20,255,20,0.5);
    -webkit-animation:blink 1.06s steps(1) infinite;
    -moz-animation:blink 1.06s steps(1) infinite;
    animation:blink 1.06s steps(1) infinite
}
.cm-animate-fat-cursor{
    width:auto;
    border:0;
    -webkit-animation:blink 1.06s steps(1) infinite;
    -moz-animation:blink 1.06s steps(1) infinite;
    animation:blink 1.06s steps(1) infinite;
    background-color:#7e7
}
@-moz-keyframes blink{
    50%{
        background-color:transparent
    }
}
@-webkit-keyframes blink{
    50%{
        background-color:transparent
    }
}
@keyframes blink{
    50%{
        background-color:transparent
    }
}
.cm-tab{
    display:inline-block;
    text-decoration:inherit
}
.CodeMirror-rulers{
    position:absolute;
    left:0;
    right:0;
    top:-50px;
    bottom:-20px;
    overflow:hidden
}
.CodeMirror-ruler{
    border-left:1px solid #ccc;
    top:0;
    bottom:0;
    position:absolute
}
.cm-s-default .cm-header{
    color:blue
}
.cm-s-default .cm-quote{
    color:#090
}
.cm-negative{
    color:#d44
}
.cm-positive{
    color:#292
}
.cm-header,.cm-strong{
    font-weight:bold
}
.cm-em{
    font-style:italic
}
.cm-link{
    text-decoration:underline
}
.cm-strikethrough{
    text-decoration:line-through
}
.cm-s-default .cm-keyword{
    color:#f19dfd
}
.cm-s-default .cm-atom{
    color:#219
}
.cm-s-default .cm-number{
    color:#164
}
.cm-s-default .cm-def{
    color:#00f
}

.cm-variable {
    color: #fded74;
}
.cm-s-default .cm-variable-2{
    color:#05a
}
.cm-s-default .cm-variable-3,.cm-s-default .cm-type{
    color:#085
}
.cm-s-default .cm-comment{
    color:#a50
}
.cm-s-default .cm-string{
    color:#fff
}
.cm-s-default .cm-string-2{
    color:#f50
}
.cm-s-default .cm-meta{
    color:#ffbaba
}
.cm-s-default .cm-qualifier{
    color:#555
}
.cm-s-default .cm-builtin{
    color:#3dc0ff
}
.cm-s-default .cm-bracket{
    color:#997
}
.cm-s-default .cm-tag{
    color:#170
}
.cm-s-default .cm-attribute{
    color:#00c
}
.cm-s-default .cm-hr{
    color:#999
}
.cm-s-default .cm-link{
    color:#00c
}
.cm-s-default .cm-error{
    color:red
}
.cm-invalidchar{
    color:red
}
.CodeMirror-composing{
    border-bottom:2px solid
}
div.CodeMirror span.CodeMirror-matchingbracket{
    color:#0b0
}
div.CodeMirror span.CodeMirror-nonmatchingbracket{
    color:#a22
}
.CodeMirror-matchingtag{
    background:rgba(255,150,0,.3)
}
.CodeMirror-activeline-background{
    background:#242F38;
}
.CodeMirror{
    position:relative;
    overflow:hidden;
    background:white
}
.CodeMirror-scroll{
    overflow:scroll !important;
    margin-bottom:-30px;
    margin-right:-30px;
    padding-bottom:30px;
    height:100%;
    outline:0;
    position:relative
}
.CodeMirror-sizer{
    position:relative;
    border-right:30px solid transparent
}
.CodeMirror-vscrollbar,.CodeMirror-hscrollbar,.CodeMirror-scrollbar-filler,.CodeMirror-gutter-filler{
    position:absolute;
    z-index:6;
    display:none
}
.CodeMirror-vscrollbar{
    right:0;
    top:0;
    overflow-x:hidden;
    overflow-y:scroll
}
.CodeMirror-hscrollbar{
    bottom:0;
    left:0;
    overflow-y:hidden;
    overflow-x:scroll
}
.CodeMirror-scrollbar-filler{
    right:0;
    bottom:0
}
.CodeMirror-gutter-filler{
    left:0;
    bottom:0
}
.CodeMirror-gutters{
    position:absolute;
    left:0;
    top:0;
    min-height:100%;
    z-index:3
}
.CodeMirror-gutter{
    white-space:normal;
    height:100%;
    display:inline-block;
    vertical-align:top;
    margin-bottom:-30px
}
.CodeMirror-gutter-wrapper{
    position:absolute;
    z-index:4;
    background:none !important;
    border:none !important
}
.CodeMirror-gutter-background{
    position:absolute;
    top:0;
    bottom:0;
    z-index:4
}
.CodeMirror-gutter-elt{
    position:absolute;
    cursor:default;
    z-index:4
}
.CodeMirror-gutter-wrapper ::selection{
    background-color:transparent
}
.CodeMirror-gutter-wrapper ::-moz-selection{
    background-color:transparent
}
.CodeMirror-lines{
    cursor:text;
    min-height:1px
}
.CodeMirror pre{
    -moz-border-radius:0;
    -webkit-border-radius:0;
    border-radius:0;
    border-width:0;
    background:transparent;
    font-family:'Source Code Pro' !important;
    font-size:inherit;
    margin:0;
    white-space:pre;
    word-wrap:normal;
    line-height:inherit;
    color:inherit;
    z-index:2;
    position:relative;
    overflow:visible;
    -webkit-tap-highlight-color:transparent;
    -webkit-font-variant-ligatures:contextual;
    font-variant-ligatures:contextual
}
.CodeMirror-wrap pre{
    word-wrap:break-word;
    white-space:pre-wrap;
    word-break:normal
}
.CodeMirror-linebackground{
    position:absolute;
    left:0;
    right:0;
    top:0;
    bottom:0;
    z-index:0
}
.CodeMirror-linewidget{
    position:relative;
    z-index:2;
    padding:.1px
}
.CodeMirror-rtl pre{
    direction:rtl
}
.CodeMirror-code{
    outline:0
}
.CodeMirror-scroll,.CodeMirror-sizer,.CodeMirror-gutter,.CodeMirror-gutters,.CodeMirror-linenumber{
    -moz-box-sizing:content-box;
    box-sizing:content-box
}
.CodeMirror-measure{
    position:absolute;
    width:100%;
    height:0;
    overflow:hidden;
    visibility:hidden
}
.CodeMirror-cursor{
    position:absolute;
    pointer-events:none
}
.CodeMirror-measure pre{
    position:static
}
div.CodeMirror-cursors{
    visibility:hidden;
    position:relative;
    z-index:3
}
div.CodeMirror-dragcursors{
    visibility:visible
}
.CodeMirror-focused div.CodeMirror-cursors{
    visibility:visible
}
.CodeMirror-selected{
    background:#d9d9d9
}
.CodeMirror-focused .CodeMirror-selected{
    background:#d7d4f0
}
.CodeMirror-crosshair{
    cursor:crosshair
}
.CodeMirror-line::selection,.CodeMirror-line>span::selection,.CodeMirror-line>span>span::selection{
    background:#d7d4f0
}
.CodeMirror-line::-moz-selection,.CodeMirror-line>span::-moz-selection,.CodeMirror-line>span>span::-moz-selection{
    background:#d7d4f0
}
.cm-searching{
    background-color:#ffa;
    background-color:rgba(255,255,0,.4)
}
.cm-force-border{
    padding-right:.1px
}
@media print{
    .CodeMirror div.CodeMirror-cursors{
        visibility:hidden
    }
}
.cm-tab-wrap-hack:after{
    content:''
}
span.CodeMirror-selectedtext{
    background:0
}

"]
        - ``````
- Copy those blocks, and then edit the css how you see fit and share it with us!
