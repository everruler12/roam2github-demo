- Designed by the Roam user community. Thanks for all your contributions! 
- Here's how to use and customize themes: 
    - {{[[youtube]]:https://youtu.be/UY-sAC2eGyI }}
- ### **Team Favorites**
    - [[Better Roam Research]]
        - If your OS is in Light Mode:
            - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FnoeJ9L0SQp.png?alt=media&token=dcfd7281-104d-4fbc-b88b-0f93de7c4f4f)
        - If your OS is in Dark Mode:
            - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FqEbHtYl5zg.png?alt=media&token=50a57675-7928-450a-b53d-23a4f5c276fc)
        - Designer::
            - Twitter:: [@linuz90](https://twitter.com/linuz90)
            - Love this theme? Say thanks via [Paypal](https://www.paypal.me/linuz90)
        - Special Features::
            - #[[Dark Mode]] but only if your OS is set to dark! 
        - Code::
            - Last updated [[June 4th, 2020]]. If it's been a while, you can check [Github](https://github.com/linuz90/better-roam-research) for the latest version. 
            - ```css
:root {
  --font-size: 15.5px;
  --border-color: rgba(0, 0, 0, 0.08);
  --subtle-border-color: rgba(0, 0, 0, 0.05);
  --main-background-color: hsl(210, 9%, 98%);
  --body-background-color: #ffffff;
  --reference-item-background: hsl(0, 0%, 99%);
  --brackets-color: rgba(0, 0, 0, 0.25);
  --empty-text-color: hsl(203, 12%, 75%); }

.rm-title-untitled,
#block-input-ghost > span,
textarea::placeholder {
  color: var(--empty-text-color) !important; }

body,
div,
textarea,
.level2 {
  font-family: 'Quattro', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif !important; }

iframe {
  border: none !important; }

.loading-astrolabe {
  position: absolute !important;
  width: 80px !important;
  height: 80px !important;
  opacity: 0.3 !important;
  top: calc(50% - 40px) !important;
  left: calc(50% - 40px) !important; }

#roam-sidebar-logo {
  display: none !important; }

body,
#app {
  background: var(--main-background-color) !important; }

.roam-center {
  border-left: 1px solid var(--border-color) !important;
  border-top: 1px solid var(--border-color) !important;
  border-right: 1px solid var(--border-color) !important;
  border-radius: 6px;
  box-shadow: 0px 2px 14px rgba(0, 0, 0, 0.04) !important;
  overflow: visible !important;
  background: var(--body-background-color) !important;
  margin-top: 10px;
  margin-right: 16px;
  margin-left: 16px; }
  .roam-center > div:first-child {
    padding-right: calc(0.5 * (100% - 820px)) !important;
    padding-left: calc(0.5 * (100% - 820px)) !important; }

.roam-topbar {
  background: var(--main-background-color) !important; }
  .roam-topbar input#find-or-create-input {
    box-shadow: none !important;
    border: 1px solid var(--border-color) !important; }

.roam-body,
.roam-topbar,
#right-sidebar,
.roam-sidebar-container {
  background: transparent !important; }

#right-sidebar {
  border: none !important;
  transition: none !important;
  overflow: hidden !important; }
  #right-sidebar h1 {
    font-size: 18px !important; }
  #right-sidebar #roam-right-sidebar-content > div[style] {
    border-bottom: 1px solid var(--subtle-border-color) !important; }
  #right-sidebar .hoverparent,
  #right-sidebar .react-resizable {
    max-width: 100% !important; }
    #right-sidebar .hoverparent img,
    #right-sidebar .react-resizable img {
      max-width: 100% !important; }

.rm-page-ref-tag {
  color: #9099a1 !important; }

span.checkmark {
  top: -2px; }

.rm-level1 div,
.rm-level1 textarea {
  font-size: 22px !important;
  line-height: 1.5 !important; }

.rm-level2 div,
.rm-level2 textarea {
  font-size: 20px !important;
  line-height: 1.5 !important; }

.rm-level3 div,
.rm-level3 textarea {
  font-size: 18px !important;
  line-height: 1.5 !important; }

.level2 {
  font-weight: inherit !important; }

.roam-log-container .roam-log-page {
  border-top: 1px solid var(--subtle-border-color) !important; }
  .roam-log-container .roam-log-page:first-child {
    min-height: 0 !important;
    border-top: none !important; }

.rm-reference-item {
  background: var(--reference-item-background) !important;
  border: 1px solid #f0f0f0 !important;
  border-radius: 6px !important;
  padding: 8px 10px 8px 2px !important; }
  .rm-reference-item .rm-block-text {
    font-size: var(--font-size) !important; }

.CodeMirror {
  font-size: 13px !important; }

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover,
.roam-body
.roam-app
.roam-sidebar-container
.roam-sidebar-content
.starred-pages-wrapper
.starred-pages
.page:hover {
  color: inherit !important;
  background-color: transparent !important; }

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper,
.roam-body
.roam-app
.roam-sidebar-container
.roam-sidebar-content
.starred-pages-wrapper
.starred-pages
.page,
.bp3-minimal > div {
  color: #666666 !important;
  font-size: 13px !important; }

.roam-sidebar-content {
  padding: 0 !important; }
  .roam-sidebar-content > div:not(.log-button):not(:first-child) {
    padding: 0 !important; }
  .roam-sidebar-content > div:first-child {
    padding-bottom: 18px !important; }

.starred-pages-wrapper > div:first-child {
  display: none; }
.starred-pages-wrapper .flex-h-box,
.starred-pages-wrapper .flex-h-box span {
  font-size: 13px !important;
  opacity: 0.6 !important; }

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button,
.roam-body
.roam-app
.roam-sidebar-container
.roam-sidebar-content
.starred-pages-wrapper
.starred-pages
.page {
  padding: 6px 24px 6px !important; }

.bp3-icon-small {
  padding-left: 24px !important; }

.rm-block-text {
  max-width: 640px !important;
  font-size: var(--font-size) !important; }

.block-bullet-view {
  margin-bottom: 3px !important; }

.roam-article > div > div h1 {
  font-size: 26px !important;
  font-weight: 700 !important;
  height: auto !important;
  line-height: 1.5 !important; }

.rm-title-display,
.rm-title-textarea {
  height: auto !important;
  line-height: 1.5 !important; }

.roam-log-container .roam-log-preview h1 {
  font-size: 22px !important;
  font-weight: 700 !important; }

strong {
  font-weight: 700 !important; }

.block-border-left {
  border-left-color: var(--subtle-border-color) !important; }

.rm-reference-main div > strong {
  color: gray !important; }

@media (prefers-color-scheme: dark) {
  body {
    background: #171717 !important; }

  #app {
    filter: invert(1) hue-rotate(180deg) !important; }

  img,
  div#buffer,
  .bp3-portal,
  .intercom-app,
  .loading-astrolabe,
  .bp3-dialog,
  .twitter-tweet,
  iframe {
    filter: invert(1) hue-rotate(180deg) !important; }

  .roam-highlight {
    background-color: #e2cb47 !important; }

  .bp3-overlay-backdrop {
    background-color: rgba(255, 255, 255, 0.7) !important; }

  :root {
    --border-color: rgba(0, 0, 0, 0.07) !important;
    --subtle-border-color: rgba(0, 0, 0, 0.05) !important;
    --main-background-color: hsl(0, 0%, 96%) !important;
    --body-background-color: hsl(0, 0%, 90%) !important;
    --reference-item-background: hsl(0, 0%, 93%) !important;
    --brackets-color: rgba(0, 0, 0, 0.3) !important;
    --empty-text-color: hsl(203, 5%, 70%); } }```
    - [[Dark Age]] 
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FSsAlUAQzX4.png?alt=media&token=cfeecde3-b93e-4422-96cf-564db274b814)
        - Designer::
            - Twitter:: [@shodty](https://twitter.com/shodty)
            - Love this theme? Say thanks via [Paypal](https://paypal.me/RobertLandsburg)
        - Special Features::
            - #[[Dark Mode]] Dark. Colorful. Smooth.
        - Code::
            - Last updated [[August 5th, 2020]].
            - **You can import the most current version of this theme with 1 line of code**
Place `@import url('https://shodty.github.io/Dark_Age.css');` inside a CSS code block on your roam/css page
            - **Include the following with your import, and easily change colors yourself!**
__Work in progress, these are the main colors, I will add all element as variables for full color customization soon!__
                ```css
@import url('https://shodty.github.io/Dark_Age.css');

  
:root {
    /* GLOBAL FONT */
    --global-font: 'Inter', sans-serif;   /* Global font (will granulate soon) */
    /* GLOBAL WIDTH FOR BLOCKS */
    --reduce-padding-right: 568px;        /* DEFAULT 568px;  Increase these two padding values to increase */
    --reduce-padding-left: 1032px;        /* DEFAULT 1032px; the global width of your blocks on the page */
    /* TEXT COLORS */
    --page-links: #D5A979;              /* [[Page Link]] */
    --attributes-color: #CEA2A1;        /* Attribute:: */
    --external-links: #53A6C8;          /* https://www.google.com */
    --links-hover: #EE8443;             /* hover color of all links */
    --hashtags: #FFFFFF84;              /* #hashtag #[[hash tags]] */
    --body-text: #FFFFFFB2;             /* general body text */
    --italics-color: #FFFFFFB2;         /* __italicized text__ */
    --bold-color: #FFFFFFB2;            /* **bolded text** */
    --highlight-text-color: #d8dadb ;   /* highlighted text color */
    --highlighter: #3b5e39;             /* highlighter color */
    --background: #26272a;              /* main page background */
    --sidebar-background: #1E1E1E;      /* sidebar background */
    --sidebar-text: #FFFFFFB2;          /* sidebar text  */
    --page-heading: #FFFFFFB2;          /* Page Title (i.e. roam/css) */
    --daily-heading: #FFFFFFB2;         /* Daily Notes date heading */
    --headings: #FFFFFFB2;              /* h1, h2, h3 */
    --bullets: #394b59;                 /* bullet color */
    --closed-bullets: #FFFFFF7C;        /* closed bullet color */
    --references: #A3B47D;              /* reference underline color */
    --block-reference-text: #A3B47D;    /* block reference color */
    --namespaces: #1CD247;              /* Namespace/color (win: ctrl+c ctrl+L) or (mac: cmd+c cmd+L) */
    --all-pages-mentions: #F79A18;      /* mentions pill on ALl Pages */
    --cursor: #FFFFFF;                  /* cursor color */
    /* ICON COLORS */ 
    --icons: #13744c;                   /* icons color */
    --icons-hover: #a06427;             /* icons hover color */
    --filter-icon: #FF0000;             /* filter icon color */
    /* FONT SIZES */
    --main-font-size: 1em;                /* DEFAULT 1em. Can change to px, e.g. 12px, or minor increments like 1.01em */
    --page-head-font-size: 36px;          /* DEFAULT 36px. page heading */
    --h1-font-size: 2em;                  /* DEFAULT 2em. h1 size */
    --h2-font-size: 1.6em;                /* DEFAULT 1.6em. h2 size */
    --h3-font-size: 1.2em;                /* DEFAULT 1.2em. h3 size */
    --sidebar-h1-size: 26px;	          /* DEFAULT 26px. sidebar page headings */
  	/* DROPDOWN MENU */
    --dropdown-menu-background: #464545; /* Dropdown menu background color */
    --dropdown-menu-highlight: #3e3d3d;  /* Dropdown menu item highlight */
    --dropdown-menu-text: #FFFFFFB2;     /* Text color in dropdown menus */
    --dropdown-newpage: #1AD546;
    /* SEARCH BAR */
    --search-bar-background: #26272a;
    --search-bar-text: #FFFFFF;
    /* KANBAN CARD COLORS */
    --kanban-main-background: #2b2a2a;
    --kanban-column-background: #2b2a2a;
    --kanban-card-background: #5959591c;
    --kanban-text-hover: #00ee6b;
}```
    - [[Leyendecker]]
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2Ffc9tIphX_X.png?alt=media&token=f6c09e01-742a-478d-a537-0b3a88796325)
        - Designer:: [[Maggie Appleton]]
            - Twitter:: [@mappletons](https://twitter.com/mappletons)
            - Love this theme? Say thanks via [Paypal](https://paypal.me/maggieappleton)
        - Special Features::
            - Queries and Kanbans got some extra love. 
            - Custom data-tags are all at the end of the CSS file, which you'll probably want to edit/customise. 
                - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FER9x_LvrLc.png?alt=media&token=4860ec31-f27e-45c7-adaa-194594cc55e2)
        - Code::
            - Last updated [[June 4th, 2020]]
            - [[Site-wide]]
                - ```css
h1,
h2,
h3,
h4,
h5,
h6 {
    font-family: "Lato", sans-serif;
    font-size: 3em;
}
div,
textarea {
    font-weight: 400;
    color: #3F4758;
    font-size: 1.002em;
}
.roam-block-container {
    max-width: 1000px;
}

.rm-pomodoro {
    background: #fff !important;
    color: #ff4747 !important;
    padding: 4px 14px;
    line-height: 2em;
    font-weight: 600;
    border-radius: 2em;
    border: 1px solid #ff474770;
}

.rm-pomodoro {
    background: #ff6956 !important;
    color: #fff !important;
    padding: 4px 14px;
    line-height: 2em;
    font-weight: 600;
    border-radius: 2em;
    border: 1px solid #ed5845;
}

.rm-pomodoro::first-letter {
  margin-right: 8px;
}

.rm-query {
    border: 0.5px solid #e4e9ec;
    border-radius: 5px;
    
}

.rm-query .rm-query-title {
    background-color: #f7f8f8;
    padding: 0.8em;
    color: #d1dbe2;
    font-size: 80%;
}

.rm-reference-main.rm-query-content {
    padding: 0.8em;
}

.rm-reference-main .rm-reference-item .rm-block-text {
    font-size: 90%;
}

.rm-ref-page-view-title span {
    
}

.rm-reference-main .rm-reference-item .controls {
    margin-left: -1em;
}

.rm-ref-page-view {
    padding: 0.4em 0.2em;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
    padding: 6px;
}

div.flex-v-box.starred-pages-wrapper > div.flex-h-box > span {
    font-size: 14px !important;
    opacity: 80%;
    letter-spacing: 0.04em;
}

div.roam-sidebar-container.noselect > div > div {
    font-size: 14px !important;
    letter-spacing: 0.03em;
    
}

#block-input {
    background: white;
}

.roam-body #block-input > span > div {
    padding: 6px 24px;
    background: white;
}

span.bp3-icon-small.bp3-icon-star {
    display: none;
    visibility: hidden;
}

.roam-block {
    max-width: 850px;
}

#right-sidebar > div {
    background-color: #f7f8fa;
    border-left: 1px solid #e9ebef;
}
.controls .simple-bullet-outer .simple-bullet-inner {
    background-color: #e5e9f2;
}
.block-border-left {
    border-left: 1px solid #f3f6f7;
}
.kanban-board {
    background-color: #fff;
}
.kanban-card {
    background-color: white;
    margin: 8px;
    box-shadow: 0px 1px 2px #9eb3c0a8;
    padding: 10px;
    border-radius: 2px;
    line-height: 1.3em;
}
.kanban-title {
    text-align: center;
    font-weight: 600;
    font-size: 1.1em;
    opacity: 80%;
    color: #485f6f;
    padding-top: 8px;
    border-bottom: 1px solid #c5d1d8;
}
.kanban-column {
    background-color: #e7eff3;
    margin: 0px 4px 0px 4px;
    padding: 4px;
    min-width: 200px;
    border-radius: 3px;
}


.rm-block-ref::before {
    content: '';
    display: inline-block;
    width: 2px;
    border-radius: 40px;
    height: 12px;
    background: #ff913c;
    margin-right: 8px;
}
.rm-block-ref {
    border-bottom: none;
    font-size: 1em;
    color: #515e70;
}
.rm-block-ref:hover {
    background: none;
    cursor: pointer;
}
.checkmark {
    background: #fff;
}
.check-container input:checked ~ .checkmark {
    background: #33bdea;
}
.check-container input:checked ~ .checkmark:after {
    border-color: #fff;
}
.rm-reference-item {
    margin-top: 8px;
    border-radius: 6px;
    border: 1px solid #e4e9ee;
    margin-right: 8px;
    flex: 1 1 100%;
    word-break: break-word;
    background-color: #f7f9fb;
    padding: 8px;
}

.rm-level2 {
    font-size: 1.5em;
}
.rm-level3 {
    color: #939aae;
    font-weight: 400;
    font-size: 1.3em;
}
.rm-page-ref {
    color: #9aabd0;
}
.rm-page-ref-link-color {
    color: #ec6f35;
    font-weight: 600;
}
a {
    color: #8A3CC8;
}
.intercom-app,
.intercom-launcher-frame,
#intercom-container {
    display: none !important;
}
.roam-body .roam-app .roam-sidebar-container {
    background-color: white;
    border-right: 1px #eee solid;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page,
.roam-body .roam-app .roam-sidebar-container > * {
    opacity: 80%;
    box-shadow: none;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
    background: white;
    color: black;
    opacity: 100%;
}
#buffer.tall {
    height: calc(100vh - 50px) !important;
}
.check-container {
    padding-right: 4px;
}
span.rm-page-ref {
    border-radius: 2px;
    padding-left: 1px;
    padding-right: 1px;
}
.content span.rm-page-ref {
    padding: 4px 1px 1px;
    /* required for fixing azo */
}
.center-proj {
    text-align: center;
}

```
            - [[Tag Styles]]
                - ```css

/* Custom data tags */
span.rm-page-ref[data-tag="Tweet"] {
    background: #81D5ED !important;
    color: white !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Literature Notes"] {
    background: #9769FF !important;
    color: white !important;
    padding: 3px 7px;
    font-weight: 500;
    line-height: 2em;
}


span.rm-page-ref[data-tag="Evergreens"] {
    background: #0DBAC6 !important;
    color: #fff !important;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Seedling"] {
    color: #0dbac6 !important;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"] {
    color: #FCB815 !important;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"]:before {
    content: '✦ '
}

span.rm-page-ref[data-tag="Illustrated Notes"] {
    color: #7172FC;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Garden Notes"] {
    color: #9DBC13;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Video Tutorial"] {
    color: #db3b8d;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Essay"] {
    background: #ADCB2A;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Livestream"] {
    color: #B979CF;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}

span.rm-page-ref[data-tag="Talk"] {
    background: #7172FC;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Waiting"] {
    background: #F9C866;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Researching"] {
    background: #FF9D66 !important;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Synthesising"] {
    background: #FC766F !important;
    color: #fff !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}


span.rm-page-ref[data-tag="Alive"] {
    background: #EE5F85 !important;
    color: #fff !important;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}```
    - [[Zenith]]
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FpF2OCzwlH2.png?alt=media&token=4bd42cd5-cd10-49a6-a915-a328ff067467)
        - Designer:: [[Azlen Elza]]
            - Twitter:: [@azlenelza](https://twitter.com/azlenelza) 
            - Love this theme? Say thanks via [Paypal](https://www.paypal.me/azlenelza). 
            - Also created "[[Cosmonaut]]" and "[[Yggdrasil]]"
        - Special Features::
            - Collapsible columns -- side-by-side view for items opened in the sidebar 
            - Searchbar appears in main page 
            - Overlay side-by-side view over graph/diagram
                - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FOAvb9EDHlf.png?alt=media&token=c0737a55-e90a-4f85-baa3-cc4797b24834)
        - Code::
            - ```css
/* IMPORT CORE THEME */
@import url('https://azlen.github.io/roam-themes/core.css');

/* GOOGLE FONTS */
@import url('https://fonts.googleapis.com/css2?family=Source+Sans+Pro:ital,wght@0,400;0,700;1,400;1,700&display=swap');	

:root {	
    --page-width: 616px;
    --page-order: row-reverse; /* new pages show up to the right */
    /*--page-order: row; /* new pages show up to the left */
    
    --header-font: "Source Sans Pro", "Inter", sans-serif;	
    --body-font: "Source Sans Pro", "Inter", sans-serif;	
    	
    --bg-color: #EEEEEE;	
    --page-color: rgba(255, 255, 255, 0.95);	
    	
    --text-color: #000000;	
    --icon-color: #5c7080;
    --bullet-color: rgba(0, 0, 0, 0.2);	
    	
    --page-shadow: 0px 8px 14px rgba(0, 0, 0, 0.05);	
    	
    --color-primary: 73, 197, 91;	
    --color-primary-contrast: #FFFFFF;	
    --color-secondary: 147, 100, 235;

    --color-secondary-contrast: #FFFFFF;	
}

/* CHANGE COLOURS IN CANVAS */
canvas[data-id="layer2-node"] {	
    filter: invert(1) hue-rotate(110deg) saturate(2.5);	
}```
- ### Dark Modes
    - [[Cosmonaut]]
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FZqga3Oe0uc.png?alt=media&token=ca5c4739-ef61-4dea-a241-eaa81a5450bf)
        - Designer:: [[Azlen Elza]]
            - "Twitter:: [@azlenelza](https://twitter.com/azlenelza) "
            - "Love this theme? Say thanks via [Paypal](https://www.paypal.me/azlenelza). "
            - Also created "[[Zenith]]" and "[[Yggdrasil]]"
        - Special Features::
            - #[[Dark Mode]]
            - Variation on [[Zenith]] which has: 
                - "Collapsible columns -- side-by-side view for items opened in the sidebar "
                - "Searchbar appears in main page "
                - "Overlay side-by-side view over graph/diagram"
        - Code::
            - ```css
/* IMPORT CORE THEME */
@import url('https://azlen.github.io/roam-themes/core.css');

/* GOOGLE FONTS */
@import url('https://fonts.googleapis.com/css2?family=Oxanium:wght@600&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Ubuntu:ital,wght@0,400;0,700;1,400;1,700&display=swap');

/* VARIABLES */
:root {
    --page-width: 616px;
    
    --header-font: "Oxanium", "Inter", sans-serif;
    --body-font: "Ubuntu", "Inter", sans-serif;
    
    --bg-color: #000000;
    --page-color: rgba(44, 44, 44, 0.95);
    
    --text-color: #FFFFFF;
    --icon-color: rgb(102, 102, 102);
    --bullet-color: rgba(255, 255, 255, 0.3);
    
    --page-shadow: 0px 8px 14px rgba(0, 0, 0, 0.25);
    
    --color-primary: 47, 155, 249;
    --color-primary-contrast: #FFFFFF;
    --color-secondary: 228, 78, 244;
    
    --color-secondary-contrast: #FFFFFF;
}

/* CHANGE COLOURS IN CANVAS */
canvas[data-id="layer2-node"] {
    filter: invert(1) contrast(1.1) hue-rotate(180deg) saturate(2);
}

/* CODE BLOCK STYLING */
/* modified from https://codemirror.net/demo/theme.html#night */
.CodeMirror { background: var(--bg-color) !important; color: #f8f8f8 !important; }
div.CodeMirror-selected { background: #447 !important;  }
.CodeMirror-line::selection, .CodeMirror-line > span::selection, .CodeMirror-line > span > span::selection { background: rgba(68, 68, 119, .99); }
.CodeMirror-line::-moz-selection, .CodeMirror-line > span::-moz-selection, .CodeMirror-line > span > span::-moz-selection { background: rgba(68, 68, 119, .99); }
.CodeMirror-gutters { background: var(--bg-color); border-right: 1px solid #252525; }
.CodeMirror-guttermarker { color: white !important; }
.CodeMirror-guttermarker-subtle { color: #bbb !important; }
.CodeMirror-linenumber { color: #f8f8f8; }
.CodeMirror-cursor { border-left: 1px solid white !important; }
span.cm-qualifier { color: #666666 !important; }
span.cm-comment { color: #C71FF9 !important; }
span.cm-atom { color: #B58AFD !important; }
span.cm-number, span.cm-attribute { color: #ffd500 !important; }
span.cm-keyword { color: #599eff !important; }
span.cm-string { color: #37f14a !important; }
span.cm-meta { color: #369BFF !important; }
span.cm-variable-2, span.cm-tag { color: #99b2ff !important; }
span.cm-variable-3, span.cm-def, span.cm-type { color: white !important; }
span.cm-bracket { color: #8da6ce !important; }
span.cm-builtin, pan.cm-special { color: #ff9e59 !important; }
span.cm-link { color: #845dc4 !important; }
span.cm-error { color: #F41000 !important; }
.CodeMirror-activeline-background { background: #1C005A !important; }
.CodeMirror-matchingbracket { outline:1px solid grey !important; color:white !important; }```
    - [[Roam Nord]] 
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FBbFviXVcSJ.png?alt=media&token=1acf0b8b-1138-41d3-a6ec-baba7e22b129)
        - Designer::
            - Twitter:: [@Elodes12](https://twitter.com/Elodes12)
            - Love this theme? To say thanks: "Make someone in your life a little bit happier if you like." 
        - Special Features::
            - #minimalist #greyscale
        - Code::
            - ```css
/*
Install theme using the Stylus extension for your web browser.
*/



.roam-block-container {
  max-width: 1000px;
}
.roam-block {
  max-width: 850px;
}


.bp3-elevation-3 {
  background-color: #434C5E !important;
}

.bp3-elevation-3 > div:hover {
  background-color: #3B4252;
}

.bp3-elevation-3 .dont-unfocus-block[style~="background-color:"] {
    background-color: #59647C !important;
}

.kanban-board {
  background-color: #fff;
}

.kanban-card {
  background-color: white;
  margin: 8px;
  box-shadow: 0px 1px 2px #9eb3c0;
  padding: 10px;
  border-radius: 2px;
  line-height: 1.3em;
}

.kanban-title {
  text-align: center;
  font-weight: bold;
  padding-top: 6px;
}

.kanban-column {
  background-color: #e4edf2;
  margin: 0px 4px 0px 4px;
  padding: 4px;
  min-width: 200px;
  border-radius: 3px;
}

.bp3-input {
    background-color: #E5E9F0
}


.rm-block-ref {
  border-bottom: none;
  font-size: 1em;
  padding: 4px;
  color: #5E81AC;
  text-decoration: underline;
}

.rm-block-ref:hover {
  background-color: #4C566A;
  color: #5E81AC;
}

.checkmark {
  background: #D8DEE9;
}
.check-container input:checked ~ .checkmark {
  background: #5E81AC;
}
.check-container input:checked ~ .checkmark:after {
  border-color: #ECEFF4;
}

.rm-level3 {
  color: #8390b2;
}

.rm-page-ref {
  color: #81A1C1;
}

.rm-page-ref-link-color {
  color: #81A1C1;
}

a {
  color: #5E81AC;
}

a:hover {
    color: #5E81AC;
}

.controls .simple-bullet-outer .simple-bullet-inner {
  background-color: #D8DEE9;
}

.rm-block-text div {
    background-color: #434C5E !important;
}


.intercom-app,
.intercom-launcher-frame,
#intercom-container {
  display: none !important;
}

.rm-reference-item div {
      background-color: #3B4252;

}

#right-sidebar div .rm-reference-item div,
.roam-topbar,
.roam-body {
  background-color: #2E3440;
}

.roam-body-main {
  background-color: #2E3440;
  color: #D8DEE9;
}

.roam-body .roam-app h1 {
  color: #E5E9F0;
}

#right-sidebar div {
  background-color: #3B4252;
}

.roam-body .roam-app .roam-sidebar-container {
  background-color: #3B4252;
  border-right: 1px #3B4252 solid;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button,
.roam-body
  .roam-app
  .roam-sidebar-container
  .roam-sidebar-content
  .starred-pages-wrapper,
.roam-body
  .roam-app
  .roam-sidebar-container
  .roam-sidebar-content
  .starred-pages-wrapper
  .starred-pages
  .page,
.roam-body .roam-app .roam-sidebar-container > * {
  opacity: 0.9;
  color: #D8DEE9;
}
.roam-body
  .roam-app
  .roam-sidebar-container
  .roam-sidebar-content
  .starred-pages-wrapper
  .starred-pages
  .page:hover,
.roam-body
  .roam-app
  .roam-sidebar-container
  .roam-sidebar-content
  .log-button:hover {
  background: #011627;
  color: #E5E9F0;
  opacity: 0.9;
}
#buffer.tall {
  height: calc(100vh - 50px) !important;
}
.check-container {
  padding-right: 4px;
}

.rm-reference-item {
  background-color: #4C566A;
}

.block-highlight-blue,
#roam-right-sidebar-content div .block-highlight-blue div {
  background-color: #4C566A;
}

.kanban-board {
    background: #011627;
    color: #E5E9F0;
}

.kanban-column {
    background-color: #c9b9bf;

}
.kanban-card{
    color: #011627;
}

/* highlights */

.roam-highlight {
    background-color: #a599e9;
}

/* reactions */

.rm-emoji-button {
    background-color: #697098 !important;
}



.rm-saving-inner-icon.rm-synced {
    background-color: #ECEFF4;
}

.rm-saving-inner-icon.rm-saving-remote {
    background-color: #5E81AC;
}

.bp3-menu {
    background-color: #E5E9F0;
}

.bp3-menu div:hover {
    background-color: #D8DEE9;
}

.bp3-button.bp3-small.block-ref-count-button {
    background-color: #D8DEE9;
    color:#2E3440;
}

.rm-reference-container .bp3-popover-target .bp3-button {
    background-color: #4C566A !important;
}


.emoji-mart {
    background-color: #E5E9F0;
}


.rm-pages-title-col {
    background-color: #4C566A;
}

.rm-pages-col {
    background-color: #4C566A;
}

.rm-pages-action-col {
    background-color: #4C566A;
}


.block-highlight-grey {
    background-color: #4C566A;
}


.CodeMirror{
    font-family: 'Dank Mono' !important;
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
    font-family:'Dank Mono';
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
    color: rgb(214, 222, 235);
}

.cm-s-default .cm-variable-2{
    color: rgb(214, 222, 235);
}
.cm-s-default .cm-variable-3,.cm-s-default .cm-type{
    color: rgb(214, 222, 235);
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
    font-family:'Dank Mono' !important;
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
}```
    - [[Apple Dark Mode]]
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FM8CxsbBexm.png?alt=media&token=938294a7-f9ff-4bd8-958b-3509a623c806)
        - Designer:: [[Bardia]]
            - Twitter:: [@thepericulum](https://twitter.com/thepericulum)
            - Love this theme? Say thanks via [Paypal](https://paypal.me/bardia95)
        - Special Features::
            - #[[Dark Mode]] #Blue
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
.intercom-app,
.intercom-launcher-frame,
#intercom-container {
    display: none !important;
}

button,
input,
optgroup,
select,
textarea,
p,
div,
h1 {
    color: white !important;
}


body {
    background: rgb(28, 28, 30) !important;
}

.roam-body .roam-app .roam-sidebar-container {
    background: rgb(28, 28, 30) !important;
}

.CodeMirror-gutters {
    background-color: rgb(72, 72, 74) !important;
    border-right: none;
}

.CodeMirror-linenumber {
    color: #8C8C8C !important;
}

.roam-block span .bp3-button {
    background: rgb(44, 44, 46) !important
}


code {
    background-color: rgb(44, 44, 46) !important;
    border: none;
    color: rgb(940, 92, 230);
    padding: .2em .4em .2em .4em;
}


.CodeMirror {
    border-radius: 8px;
    background-color: rgb(44, 44, 46) !important;
    color: white !important;
}

.cm-s-default .cm-keyword,
.cm-atom {
    color: rgb(191, 90, 242) !important;
}

.cm-s-default .cm-builtin {
    color: rgb(10, 132, 255) !important;
}

a {
    color: rgb(255, 159, 10);
}

a:hover {
    color: rgb(255, 159, 10);
}

.rm-level1 .checkmark {
    top: -3px;
}


.parent-path-wrapper {
    background: rgb(28, 28, 30) !important;
}

.rm-saving-icon .rm-synced {
    background: rgb(48, 209, 88) !important;
}

.check-container input:checked ~ .checkmark {
    background-color: rgb(10, 132, 255) !important;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover {
    color: rgb(191, 90, 242) !important;
    background: rgb(28, 28, 30) !important;
}


.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
    font-size: 15px;
    font-weight: 500 !important;
}

body {
    font-size: 1.2em;
}


h1 > a {
    color: rgb(100, 210, 255) !important;
}
a > span {
    color: rgb(100, 210, 255) !important;
}

.rm-page-ref-link-color {
    color: rgb(100, 210, 255) !important;
}

#roam-right-sidebar-content .bp3-button {
    background: rgb(44, 44, 46) !important;
}

.rm-reference-item {
    background-color: rgb(44, 44, 46);
    padding: 5px;
    border-radius: 7px;
}

#roam-sidebar-logo:hover {
    color: white;
    text-decoration: none;
    background: rgb(28, 28, 30) !important;
}

#roam-sidebar-logo {
    text-decoration: none;
}

.katex * {
    color: rgb(191, 90, 242) !important;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
    color: rgb(191, 90, 242) !important;
    background: rgb(28, 28, 30) !important;
}

.roam-body-main #right-sidebar {
    background-color: rgb(44, 44, 46) !important;
}

.bp3-elevation-3 {
    background-color: rgb(44, 44, 46) !important;
}

.bp3-elevation-3 > .dont-unfocus-block {
    filter: invert(100%);
    /*RR change: Inverts the colors of the / and link search menus*/
}

.bp3-text-overflow-ellipsis {
    color: black !important;
}

#roam-right-sidebar-content > div {
    border-bottom: none !important;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page,
.roam-body .roam-app .roam-sidebar-container > * {
    color: white !important;
}


.flex-v-box.starred-pages-wrapper > div:first-of-type {
    opacity: 0;
}


.log-button {
    color: white !important;
}


.check-container {
    padding-right: 4px;
}

.rm-page-ref-brackets {
    opacity: .3;
}

/* .starred-pages-wrapper:first-child { } */
.bp3-input {
    box-shadow: none;
    border: 1px solid #73869447 !important;
}

.roam-log-container .roam-log-page {
    border-top: 0px solid #73869447 !important;
    margin-top: 0px;
}

.rm-level1,
.rm-level2 {
    font-weight: 600;
}

.rm-level1 {
    font-size: 1.6em;
}
.rm-level2 {
    font-size: 1.2em;
}

.block-border-left {
    border-left: 1px solid #bfccd690;
    /* Lighten */
}

.katex .fontsize-ensurer.reset-size6.size3,
.katex .sizing.reset-size6.size3 {
    font-size: .7em !important;
}
.rm-reference-item {
    margin-top: 0;
}

.bp3-popover-content > div {
    max-height: 520px !important;
}

.h1,
.h2,
.h3,
.h4,
.h5,
.h6,
h1,
h2,
h3,
h4,
h5,
h6,
textarea,
div {
    font-family: 'Helvetica Neue' !important;
    font-weight: 400 !important;
}

.h3,
h3,
.rm-level3 span {
    color: rgb(48, 209, 88) !important;
}

.h2,
h2,
.rm-level2 {
    font-size: 1.3em !important;
}

textarea,
span {
    letter-spacing: 0.02em !important;
}

.katex .msupsub {
    font-size: .8em !important;
}

.log-button,
.log-button .flex-h-box {
    font-weight: 700 !important;
}

.roam-sidebar-container {
    box-shadow: none !important;
    width: 13vw !important;
    min-width: 200px;
}

.roam-body-main {
    height: 100% !important;
    top: 0 !important;
}

.roam-topbar {
    opacity: 0;
    transition: opacity 200ms;
    z-index: 1;
    background: none;
    /* Making space for the close sidebar button */
    width: calc(100% - 40px);
    padding: 0;
}

.roam-topbar:hover,
.roam-topbar:focus-within {
    opacity: 1;
    transition: opacity 200ms;
}

.roam-log-container .roam-log-page {
    border-top: 1px solid #00000048;
}

#right-sidebar button {
    z-index: 100000;
}

hr .roam-center .bp3-button.bp3-small.block-ref-count-button {
    background: white !important;
}


/* Hide "Starred" header */
.flex-v-box.starred-pages-wrapper > .flex-h-box {
    display: none;
}

.roam-right-sidebar-content div div {
    margin-left: -8px !important;
    margin-right: -8px !important;
}

#right-sidebar .rm-reference-item {
    background-color: rgb(28, 28, 30);
}

.rm-reference-item {
    margin-bottom: 10px;
}

strong {
    color: rgb(10, 132, 255) !important;
}

.roam-highlight,
.roam-highlight strong {
    background-color: rgb(255, 214, 10);
    color: rgb(28, 28, 30) !important;
}

.roam-highlight .rm-page-ref {
    color: rgb(10, 132, 255) !important;
}

.block-highlight-yellow {
    background-color: #8C8C8C !important;
}

.roam-bullet-closed {
    background-color: rgb(10, 132, 255) !important;
}

.simple-bullet-inner {
    background-color: rgb(100, 210, 255) !important;
}

.rm-page-ref-tag {
    color: rgb(255, 55, 95);
}

.bp3-button.bp3-minimal.bp3-small {
    margin-right: 4px;
    margin-left: -4px;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .bp3-button[class*="bp3-icon-"]::before {
    color: white;
}

.controls {
    padding-top: 5px !important;
}

.rm-page-ref {
    font-size: 1em !important;
}

.check-container {
    padding-top: 1px;
}


/* Hide help button */
#buffer {
    visibility: hidden;
}```
    - Dark Roam 
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FJFROdH1eNh.png?alt=media&token=9d012c48-3515-4242-bfb1-cea730f6d7a4)
        - Designer:: [[Ryan Rich]]
            - Twitter:: [@rrichrs](https://twitter.com/rrichrs)
            - Love this theme? Say thanks via [Paypal](https://paypal.me/rrichrs) or [buy him a coffee](https://www.buymeacoffee.com/rrichrs). 
        - Special Features::
            - #[[Dark Mode]]
        - Code::
            - Last updated [[June 4th, 2020]]. You can check [Github](https://gist.github.com/rr1000/eedbd56e55d132c1779445c70a1c011d) for the latest version. 
            - ```css
body {
     color: #fff;
}
 .roam-article {
     color: #fff;
}
 .rm-page-ref-link-color {
     color: #fff;
     text-decoration: underline;
}
 .controls .simple-bullet-outer .simple-bullet-inner {
     background-color: #ddd;
}
 .controls .simple-bullet-outer {
     color: #ddd;
}
 .rm-page-ref-link-color:hover {
     color: #ddd;
}
 .roam-body {
     background-color: #2F3437;
}
 .roam-topbar {
     background-color: #2F3437;
}
 .roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button {
     color: #ddd;
}
 .roam-sidebar-content {
     background-color: #373C3F;
}
 .roam-body .roam-app h1 {
     color: #fff;
}
 .starred-pages-wrapper .flex-h-box span {
     color: #ddd;
}
 .roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
     color: #fff;
}
 .bp3-input {
     color: #fff;
     background-color: #2F3437;
     border: 1px solid rgba(255, 255, 255, 0.2);
}
 body a {
     color: #4fb6ff;
}
 .rm-saving-icon .rm-synced {
     color: #5dff8f;
}
 .rm-reference-item {
     background-color: #373C3F;
     border-radius: 5px;
}
 code {
     color: #ff57d3;
     background: #252525;
     border: 0;
}
 .roam-body-main #right-sidebar {
     background-color: #373C3F !important;
}
 .roam-body .roam-app {
     color: #fff;
}
 .roam-block-container .bp3-elevation-3 {
     background-color: #373C3F !important;
}
 .rm-level3 {
     color: #65d88e;
}
 .bp3-popover .bp3-popover-content{
     background: #464b4e;
}
 .bp3-popover-content .bp3-button:not([class*="bp3-intent-"]){
     background-color: #8ea2af;
     background-image: -webkit-gradient(linear,left top,left bottom,from(rgba(255,255,255,0.8)),to(rgba(255,255,255,0)));
     background-image: linear-gradient(to bottom,#d3eaf9,rgba(255,255,255,0));
     -webkit-box-shadow: inset 0 0 0 1px rgba(16,22,26,0.2), inset 0 -1px 0 rgba(16,22,26,0.1);
     box-shadow: inset 0 0 0 1px rgba(16,22,26,0.2), inset 0 -1px 0 rgba(16,22,26,0.1);
     color: #182026;
}
 .bp3-popover .bp3-popover-arrow-fill {
     fill: #2f3537;
}
 .bp3-menu{
     background-color: #2f3537;
}
 .bp3-menu-item{
     color: #fff;
}
 .bp3-menu-item:hover{
     color: #ddd;
}
 .rm-pages-row {
     display: flex;
     flex: 0 0 auto;
     justify-content: space-between;
     align-items: flex-start;
     margin-bottom: 10px;
     border-radius: 5px;
     padding: 5px;
     border: 1px solid #171f21;
     background-color: #39525a !important;
}
 .bp3-text-overflow-ellipsis a{
     color: #fff !important;
}
 .bp3-button.bp3-minimal.bp3-intent-success {
     color: #50ffb6;
     background-color: #2e5a4e;
}```
    - Roam Gotham
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2F1gT_TuyMlm.png?alt=media&token=c9e654da-8251-474f-85ac-b2883ab1ddb3)
        - Designer::
            - Twitter:: [@adityadaniel](https://twitter.com/adityadaniel)
            - Love this theme? Say thanks via [Paypal](https://www.paypal.me/adityadaniel)
        - Special Features::
            - #[[Dark Mode]] #green 
Based on Bear Gotham theme
        - Code::
            - ```css
body {
    font-size: 16px;
    font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
    letter-spacing: -0.001em;
    line-height: 1.5;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
}

@media (prefers-color-scheme: dark) {
    .roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button {
        padding: 8px 20px;
        font-weight: 900;
        cursor: pointer;
        font-size: 16px;
        color: #2eb88c;
    }


    /* Background color for the rest of body */
    body {
        background-color: #11151c;
        font-size: 16px;
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
        letter-spacing: -0.001em;
        line-height: 1.5;
        -webkit-font-smoothing: antialiased;
        text-rendering: optimizeLegibility;
    }

    /* Header - Note title */
    .roam-app h1 {
        color: #2eb88c !important;
        font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif, "Apple Color Emoji", "Segoe UI Emoji", "Segoe UI Symbol";
        font-weight: bold;
    }

    /* primary text colour */
    .roam-app {
        color: #6aa9b9 !important;
    }

    /*topbar*/
    .roam-topbar {
        background-color: #11151c;
        border-bottom: 1px solid #1c373e;
    }

    /*sidebar*/
    .roam-body .roam-app .roam-sidebar-container {
        background-color: #11151c;
        border-right: 1px solid #1c373e;
    }

    .roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper {
        color: #2eb88c;
    }

    .flex-v-box .starred-pages-wrapper:first-child {
        background-color: #1c373e;
    }

    .roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
        color: #2eb88c
    }

    .roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover {
        color: white;
    }

    /*right sidebar*/
    #right-sidebar {
        background-color: #11151c !important;
        border-left: 1px solid #1c373e;
        font-size: 15px;
    }

    #right-sidebar .flex-h-box .bp3-button .bp3-minimal .bp3-small {
        color: #2eb88c;
    }

    /*border between page in daily notes*/
    .roam-log-container .roam-log-page {
        border-top: 1px solid #1c373e;
    }

    /* hashtags */
    .rm-page-ref-tag {
        color: #d4fef0 !important;
        background: #1a6950;
        padding: .1em .6em;
        border-radius: 12px;

    }

    .block-border-left {
        border-left: 1px solid #1c373e;
    }

    .rm-block-ref {
        border-bottom: 1px solid #2eb88c;
    }

    .rm-block-ref:hover {
        background: #091722;
        border: 1px solid #112a3f;
    }

    .rm-page-ref-tag:hover {
        text-decoration: underline;
    }

    /* the bright blue highlight color */
    .block-highlight-blue {
        background-color: #1c2e3e;
    }

    /* the reference boxes at the bottom */
    .rm-reference-item {
        background-color: #0B1721;
        margin-top: 12px;
        border: 1px solid #1E3745;
        border-radius: 4px;
    }

    .rm-reference-item .roam-block {
        padding-top: 8px;
        padding-bottom: 8px;
    }

    .rm-reference-item .controls {
        padding-top: 10px;
        padding-bottom: 4px;
    }

    .rm-page-ref.rm-page-ref-link-color {
        color: #f2825a;
    }

    .rm-page-ref:hover {
        color: #ff895e;
    }

    .rm-page-ref.rm-page-ref-link-color {
        color: #f2825a;
    }

    a {
    color: #f2825a;
    }

    a:focus {
        color: #f2825a;
    }

    a:hover {
        color: #ff895e;
    }

    .rm-level2 {
        color: #2eb88c;
        font-weight: 700;
    }

    .rm-level3 {
        color: #2eb88c;
        font-weight: 500;
    }

    code {
        color: #a0a2b6;
        background: #091722;
        border: 1px solid #112a3f;
        padding: 0.3em 0.4em;
        border-radius: 3px;
    }


    /* CodeMirror */
    .CodeMirror {
        background: #091722;
        color: #589cab;
    }

    .CodeMirror-lines {
        color: #a0a2b6
    }

    .CodeMirror-gutters {
        background-color: #091722;
        border-right: 1px solid #112a3f;
    }

    .CodeMirror-activeline-background {
        background: #0D2030;
    }

    .cm-s-default .cm-keyword {
        color: #5393a2;
    }

    .cm-s-default .cm-bracket .CodeMirror-matchingbracket {
        text-decoration: #5393a2;
        color: white !important;
    }

}```
    - Spotify
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FLTmmrGuk7l.png?alt=media&token=1de7f1b6-f0eb-440a-b567-d1e53e46e8f0)
        - Designer:: [[Aaron Lewis]]
            - Twitter:: @aaronzlewis
            - Love this theme? Say thanks via [Paypal](https://paypal.me/aaronzlewis)
        - Special Features:: 
            - #[[Dark Mode]]
            - Elegant solution to embedding block references — an old typographical symbol (the Guillemet) that indicates a quote. 
            - Easy to scan linked references. 
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
body {
    font-size: 15px;
    letter-spacing: -0.001em;
    line-height: 1.5;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
}


.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button {
    padding: 8px 20px;
    font-weight: 900;
    cursor: pointer;
    font-size: 14px;
    color: #8F9294;
}

.roam-block-container {
  max-width: 600px;
}
.roam-block {
  max-width: 600px;
}

.check-container input:checked ~ .checkmark {
  background: #65D36E;
}


.bp3-button.bp3-minimal.bp3-intent-success {
    color: #65D36E;
}

.bp3-button.bp3-minimal.bp3-intent-success:hover {
    color: #65D36E;
    background-color: #E4E5EA;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
    background-color: #282828;
    color: #65D36E;
}


/* Background color for the rest of body */
body {
    background-color: #181818;
    font-size: 15px;
    letter-spacing: -0.001em;
    line-height: 1.5;
    -webkit-font-smoothing: antialiased;
    text-rendering: optimizeLegibility;
}

h1, 
h2,
h3,
h4,
h5,
h6,
textarea,
div {
    color: white;
    font-family: 'SF Pro Text';
}

h3, h3 textarea {
    font-weight: 700 !important;
    font-size: 12px !important;
    text-transform: uppercase !important;
    letter-spacing: 0.01em;
} 

.rm-alias-external {
    color: #73AEEA;
    text-decoration: underline;
}

.rm-alias-external:hover {
    text-decoration: none;
    color: #73AEEA;
}




/* Header - Note title */
.roam-app h1, .rm-title-display span, .roam-app h1 textarea {
    font-family: "Poppins" !important;
    font-size: 28px;
    font-weight: 800;
    line-height: 110%;
    color: white !important;
}

/* primary text colour */
.roam-app {
    color: #000 !important;
}

.bp3-button.bp3-small, .bp3-small .bp3-button {
    color: #181818 !important;
}

/*topbar*/
.roam-topbar {
    background-color: #181818;
 
}

.rm-search-title {
    color: black !important;
}

.bp3-menu-item >.bp3-fill {
    color: black !important;
}

.bp3-elevation-3 {
    background-color: #282828 !important;
    padding: 8px !important;
    border-radius: 8px;
    box-shadow: 0px 4px 32px rgba(0,0,0,0.2);
}

.bp3-elevation-3 div { 
  color: #8F9294 !important;
}

/*sidebar*/

.starred-pages-wrapper {
    border: none !important;
}

.roam-body .roam-app .roam-sidebar-container {
    background-color: #282828;

 
}

.log-button {
    font-weight: 700 !important;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper {
    color: #8F9294;
}

.flex-v-box .starred-pages-wrapper:first-child {
    background-color: #8F9294;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
    color: #8F9294;
    font-weight: 500;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover {
    color: #65D36E;
    background-color: #282828;
}

/*right sidebar*/
#right-sidebar {
    box-shadow: -4px 0px 15px 3px rgba(0,0,0,0.02);
    background-color: #282828 !important;
}

#right-sidebar h1 {
    font-family: BlinkMacSystemFont;
    font-weight: 600;
    font-size: 20px;
    line-height: 130%;
    padding: 8px 0px;
    
}

#right-sidebar h1 a {
    color: white !important;
}

#right-sidebar .flex-h-box .bp3-button .bp3-minimal .bp3-small {
    color: #73AEEA;
}

/*border between page in daily notes*/
.roam-log-container .roam-log-page {
    border-top: 1px solid rgba(255,255,255,.1)
}

.intercom-app,
.intercom-launcher-frame,
#intercom-container {
  display: none !important;
}

.check-container {
  padding-right: 4px;
}

.bp3-button {
    color: white !important;
}

/* hashtags */
.rm-page-ref-tag {
    color: #999;
    font-weight: 500;
    padding: 0em .2em;
    border-radius: 4px;
}

.block-border-left {
    border-left: 1px solid rgba(255,255,255,0.12);
}


.rm-block-ref:hover {
   text-decoration: underline;
   background: none;
   cursor: pointer;
}

.rm-block-ref {
    font-size: 15px;
    border-bottom: none;
    color: white;
}

.rm-block-ref::before {
    content: '»';
    font-size: 15px;
    font-weight: 500;
    color: #65D36E;
    display: inline-block;
    margin-right: 4px;
}

.roam-highlight {
    background: rgba(255, 255, 0, 0.2);
}

.rm-page-ref-tag:hover {
    text-decoration: underline;
}

.rm-encrypted-block {
    font-size: 15px;
    background-color: #282828;
    font-weight: 400;
}

.roam-block-container, .rm-block-input {
  max-width: 600px;
}
.roam-block {
  max-width: 600px;
}

.rm-embed-container {
    background-color: #121212;
    padding: 12px;
    border-radius: 4px;
}

/* the bright blue highlight color */
.block-highlight-blue {
    background-color: rgba(255,255,255,0.08);
}

/* the reference boxes at the bottom */
.rm-reference-item {
    background-color: rgba(255,255,255,0.03);
    padding: 12px 20px 12px 0px;
    border-radius: 4px;
    border: 1px solid rgba(255,255,255,0.04);
    margin-bottom: 4px;
}

.rm-page-ref.rm-page-ref-link-color {
    color: #65D36E;
    font-weight: 600;
}


a {
    color: #65D36E;
}

a:focus {
    color: #65D36E;
}

a:hover {
    color: #65D36E;
}

.rm-level2 {
    color: #65D36E;
    font-weight: 600;
}

.rm-title-arrow-wrapper {
    margin-top: 20px;
}

.rm-ref-page-view-title a {
    color: #73AEEA !important;
    font-weight: 700;
    font-size: 15px;
    line-height: 140%;
    margin-top: 12px;
    margin-bottom: 4px
}

.kanban-board {
  background-color: rgba(255,255,255,0);  
  width: 130%;
}

.bp3-button.bp3-small, .bp3-small .bp3-button {
    color: white !important;
}


.kanban-card:hover {
    background-color: #484C50;
}

.kanban-card, foreignObject {
  box-shadow: 0px 1px 4px rgba(0,0,0,0.08);
  border-radius: 6px;
}

.kanban-card {
  font-size: 12px;
  background-color: #404447;
  margin: 8px 12px;
  padding: 12px;
}

.kanban-title {
  text-align: center;
  padding-top: 8px;
  border-bottom: 1px solid #444;
  text-transform: uppercase;
  font-size: 12px;
  font-weight: 900;
}

.kanban-column {
  background-color: #282828;
  margin: 0px 4px 0px 4px;
  padding: 4px;
  min-width: 200px;
  border-radius: 4px;
}

.kanban-column:active, .kanban-column:focus, .kanban.column:hover, .kanban.column:enabled {
    background-color: #383838 !important;
}```
- ### Feature Expansions
    - Nested Links
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2Fqr3tGRCd-s.png?alt=media&token=31913a3e-546a-4955-87fe-2c9ad8fd160f)
        - Designer::
            - Twitter:: [@CatoMinor3](https://twitter.com/CatoMinor3)
            - Love this theme? Say thanks via [Paypal](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=6AMGMUDRX29XU&source=url)
        - Special Features::
            - Additional underlining for nested tags 
                - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FNRBiiUtnF-.png?alt=media&token=233612e7-2aeb-4d13-b28e-8b9cc806d173)
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
:root {
    --custom-background-color: lightsteelblue;
    --custom-background-color-hover: orange;
    }


.rm-page-ref-link-color{
   color:black !important;
    background: linear-gradient(0deg, var(--custom-background-color) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
    line-height: 24px;
    padding-bottom: 4px;
}

.rm-page-ref-link-color:hover{
   color:black !important;
    background: linear-gradient(0deg, var(--custom-background-color-hover) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
    text-decoration: none;
    line-height: 24px;
    padding-bottom: 4px;
}

.rm-page-ref-link-color .rm-page-ref-link-color {
color: black !important;
  background: linear-gradient(0deg, var(--custom-background-color) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
   line-height: 28px;
    padding-bottom: 8px;
}

.rm-page-ref-link-color .rm-page-ref-link-color:hover {
color: black !important;
  background: linear-gradient(0deg, var(--custom-background-color-hover) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
   line-height: 28px;
    padding-bottom: 8px;
}


.rm-page-ref-link-color .rm-page-ref-link-color .rm-page-ref-link-color {
color: black !important;
background: linear-gradient(0deg, var(--custom-background-color) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
   line-height: 32px;
    padding-bottom: 12px;
}


.rm-page-ref-link-color .rm-page-ref-link-color .rm-page-ref-link-color:hover {
color: black !important;
background: linear-gradient(0deg, var(--custom-background-color-hover) 2px, white 1px, transparent 1px);
    background-position: 0 100%;
   line-height: 32px;
    padding-bottom: 12px;
}```
    - Right to Left
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Fhelp%2FiNm7LrjEBx.png?alt=media&token=9aaadf79-c0fd-466e-ba4d-c8f49e7144f7)
        - Designer:: [[David Crandall]]
            - Twitter:: [@davidcrandall_w](https://twitter.com/DavidCrandall_W)
            - Love this theme? Say thanks via [Paypal](https://paypal.me/davidcrandallwrites)  
            - Also created: "Split Screen" 
        - Special Features::
            - This theme provides support for right to left (RTL) languages like Hebrew and Arabic.
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
/* Right to Left CSS for Roam                */
/* "Assembled" and tweaked by @DavidCrandall */
/* https://davidcrandallwrites.com           */



.roam-body .roam-app .roam-sidebar-container {
    right: -232px;
    /* left: 0px; */
}
.roam-body-main .flex-h-box {
    direction: rtl;
}

.roam-sidebar-container {
    direction: rtl;
}

.flex-v-box {
    margin-left: 0px !important;
    margin-right: 20px;
}

.scrollbar {
    margin-left: 0px;
    margin-right: 30px;
    float: right;
}

#home .icons .bp3-icon-large:hover {
    margin-left: 0px;
    margin-right: 60px;
}

#landing-page #cover #tag-line ul {
    margin-right: 32px;
    margin-left: 16px;
}
#landing-page #cover #endorsement {
    margin: 80px 20px 20px;
}
#landing-page #features ul {
    padding-left: 0px;
    padding-right: 16px;
}
.rm-emoji-block-view {
    margin-left: 0px;
    margin-right: 40px;
}

@media (max-width: 500px) {
    .bp3-omnibar {
        max-width: 310px;
        right: calc((100vw - 310px) / 2);
    }
}
.roam-topbar {
    padding-left: 16px;
    padding-right: 16px;
}
.check-container {
    padding-left: 0px;
    padding-right: 12px;
}
/* Create a custom checkbox */
.checkmark {
    right: 0;
}
.rm-title-display {
    direction: rtl;
}
/* Style the checkmark/indicator */
.check-container .checkmark:after {
    right: 3.5px;
}
.rm-find-or-create-wrapper .rm-menu-item .rm-search-list-item {
    margin-left: 0px;
    margin-right: -20px;
}
.rm-pages-sort-menu-item {
    padding-left: 16px;
    padding-right: 16px;
}
.rm-histogram-table {
    margin-right: -8px;
}
#right-sidebar .roam-bullet-closed {
    background-color: #a7b6c2;
}
#mobile-capture li div {
    margin-left: 0px;
    margin-right: 12px;
}
.edited-by-view {
    margin-left: 0px;
    margin-right: 0px;
}
.block-bullet-view {
    margin-left: 0px;
    margin-right: 5px;
}
.block-border-left {
    border-left: 0px;
    border-right: 1px solid #bfccd6;
    /* #bfccd6;*/
}
.text-align-left {
    text-align: right;
}
.text-align-right {
    text-align: right;
}
.controls {
    padding-left: 0px;
    padding-right: 4px;
}
.version-bullet {
    margin-left: 0px;
    margin-right: 0px;
}
.dnd-separator .dnd-drop-bar {
    right: 20px;
}
.tags-input {
    text-align: right;
}
.tags-output {
    margin-left: 0px;
    margin-right: 4px;
}
.tags-output-item2 {
    margin-left: 0px;
    margin-right: 6px;
}```
    - Split Screen
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FbOv86UR_Ir.png?alt=media&token=aa25fa62-5995-404e-9b79-4409c436e4aa)
        - Designer:: [[David Crandall]]
            - "Twitter:: [@davidcrandall_w](https://twitter.com/DavidCrandall_W)"
            - "Love this theme? Say thanks via [Paypal](https://paypal.me/davidcrandallwrites)  "
            - Also created: "Right to Left"
        - Special Features::
            - This theme gives the sidebar equal width with the main writing area, while decreasing the darkness of the background to make for a more comfortable writing area. 
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
"/* Split Screen CSS for Roam */
/* "Assembled" and tweaked by @DavidCrandall */
/* https://davidcrandallwrites.com */


/* change main font */

body,
html,
div,
textarea {
font-family: -apple-system, BlinkMacSystemFont, sans-serif;
}

/* change font for all headings */

h1,
h1 div,
h1 textarea,
.rm-level1 div,
#right-sidebar .rm-level2, /* page headings in right sidebar */
.rm-reference-main .rm-level3 , /* page headings in referenced items */
.rm-level1 textarea,
.roam-log-preview h1,
h1.rm-title-display,
h1.rm-title-display textarea,
.level1,
.level2 {
--font-family: "Fira Code", Menlo, monospace;
font-family: -apple-system, BlinkMacSystemFont, sans-serif;
font-weight: 500 !important;
--letter-spacing: -0.08em;
}

h2,
h2 div,
h2 textarea,
h3,
h3 div,
h3 textarea {
--font-family: "Fira Code", Menlo, monospace;
font-family: -apple-system, BlinkMacSystemFont, sans-serif;
color: #333 !important;
}

a {
color: #106ba3;
/* #4f718f; */
}

/* less space below page heading */

.roam-body .roam-app .roam-main .roam-article .rm-title-display {
margin-bottom: 10px;
}


h1.level2 {
font-size: 36px !important;
}

/* Main block - remove centering */

.roam-center {
--align-item: left;
flex-basis: 40% !important;
}



/* lighter bullets */

#right-sidebar .controls .roam-bullet-closed,
.controls .roam-bullet-closed {
background: none;
border: 1px solid silver;
}

.simple-bullet-inner {
opacity: 0.3;
}

/* lighter vertical guides */

.block-border-left {
border-color: #eee;
}


.roam-block-container h1 {
font-weight: 300;
font-size: 26px;
color: black;
}

.roam-block-container h2 {
font-weight: 600;
font-size: 18px;
color: black;
}

/* align checkboxes better */

label.check-container {
margin-bottom: 11px;
margin-right: 3px;
}

/* align checkboxes in zoomed-in headings */

.rm-level1 label.check-container {
margin-bottom: 17px;
margin-right: -3px;
}

/* don't shrink block references */

.rm-block-ref {
font-size: 1em;
padding: 0;
margin: 0;
}

.rm-block-ref label.check-container {
margin-bottom: 12px;
}



/* don't need "SHORTCUTS" heading */

.starred-pages-wrapper .flex-h-box {
display: none;
}

.starred-pages-wrapper > div:first-child {
margin: 0 -18px;
}

/* more subtle logo */

#roam-sidebar-logo img {
opacity: 0.4;
}
#roam-sidebar-logo span {
display: none;
}

/* fade loading astrolabe */

.loading-astrolabe img {
opacity: 0.2;
}

/* lighter sidebar background */

#right-sidebar {
background-color: rgba(216, 225, 232, 0.2) !important;
/* rgba(216, 225, 232, 0.3) */
border-left: 1px solid #ddd !important;
}

/* sidebar sections */

#roam-right-sidebar-content > div {
border-bottom: 1px solid #ddd !important;
margin: 0 !important;
padding: 10px 4px 10px 50px;
}

/* sidebar section headings */

#roam-right-sidebar-content > div > div:first-child {
margin-left: -10px;
}

/* rule under top section of left sidebar */

.roam-sidebar-content > div:first-child {
padding: 4px 16px !important;
margin-bottom: 8px;
border-bottom: 1px solid rgb(57, 75, 89);
}

/* rule under topbar */

.roam-topbar {
border-bottom: 1px solid #eee;
}

/* crumbs */

.rm-reference-item
> div:first-child
> div:first-child
div
span:not(.bp3-icon-chevron-right),
.roam-article
> div:first-child:not(.roam-log-container)
> div:first-child
div
span:not(.bp3-icon-chevron-right) {
font-size: 12px;
line-height: 1.3;
color: #bbb !important;
/* truncate to smaller width, use css for ellipsis */
--max-width: 1000px;
white-space: nowrap;
overflow: hidden;
text-overflow: ellipsis;
padding: 2px !important;
}

.rm-reference-item
> div:first-child
> div:first-child
div
span:hover:not(.bp3-icon-chevron-right),
.roam-article
> div:first-child:not(.roam-log-container)
> div:first-child
div
span:hover:not(.bp3-icon-chevron-right) {
color: black !important;
}

/* chevrons in crumbs */

.roam-reference-item > div > div:first-child .bp3-icon-chevron-right,
.roam-article
> div
> div:first-child:not(.roam-log-container)
.bp3-icon-chevron-right {
font-size: 1em;
margin: 0 3px;
color: #ddd !important;
}

/* no checkboxes in crumbs */

.roam-reference-item
> div:first-child:not(.roam-log-container)
> div:first-child
label.check-container,
.roam-article
> div:first-child:not(.roam-log-container)
> div:first-child
label.check-container {
display: none;
}

/* link buttons for referenced items */

.rm-reference-main button {
border: 1px solid #eee;
border-radius: 0.3em;
font-size: 0.8em;
}

.rm-reference-main button:hover {
border-color: #ccc;
}

/* referenced item section headings */

.rm-reference-main {
--border-top: 1px solid #ededed;
}

.flex-h-box {
padding-top: 0px !important;
}

.rm-reference-main .flex-h-box {
min-height: 30px;
}

.rm-reference-main strong {
color: #666;
font-size: 0.8em;
--background-color: rgba(216, 225, 232, 0.3);
}

/* remove background from referenced items */

.rm-reference-item {
padding: 6px 0 0 0;
margin: 6px 0 0 0;
border-top: 1px solid #eee;
background: none;
}

/* slightly bigger page headings under referenced items */
.rm-reference-main .rm-level3 {
font-size: 1.6em;
}

/* search */

.rm-find-or-create-wrapper {
flex: 0 1 100% !important;
}

.rm-find-or-create-wrapper .bp3-input {
border: none !important;
box-shadow: none !important;
}

/* highlights */

.roam-highlight {
--background-color: #c2f9fa;
}

/* links */

a.rm-alias.rm-alias-external {
color: #b33ba9 !important;
}

.rm-page-ref-link-color {
color: #106ba3;
}	```
    - Split Tags
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2Fi_PJGC0DcZ.png?alt=media&token=fb549b9f-7b25-42e0-ac01-1349eb284b69)
        - Designer:: [[Gary Basin]]
            - Twitter:: [@garybasin](https://twitter.com/garybasin)
            - Love this theme? Say thanks via [Paypal](http://paypal.me/garybasin)
        - Special Features::
            - Add-on to "Split Screen" by [[David Crandall]] 
            - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FJu6Mc0kNw9.png?alt=media&token=e4125542-95fc-461f-9dd9-5316eb9e493a)
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
/* Split Screen CSS for Roam                 */
/* "Assembled" and tweaked by @DavidCrandall */
/* https://davidcrandallwrites.com           */
/* https://davidcrandallwrites.com/split-screen-and-rtl-custom-css-scripts-for-roam/ */
/*                                           */
/* Added tags by @garybasin                  */


/* tags */

.rm-page-ref-tag {
    font-size: 0.8em;
    font-weight: bold;  
    padding: 6px;
    margin: 4px;
    border-radius: 5px;
    border: 1px #bdbdbd dotted;
}

[data-tag="me"] {
    /* Styles */
    color: #000;
    background-color: #c9e33e;
}

[data-tag="ps"] {
    color: white;
    background-color: #5353ff;
}

[data-tag="kap"] {
    color: white;
    background-color: #ff5f5f;
}

[data-tag="Sini"] {
    color: white;
    background-color: #55993a;
}

[data-tag="Roam-Highlights"] {
    color: #b7b7b7;
    background-color: #ffffb4;
}

/****************************/

/* change main font */

body,
html,
div,
textarea {
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
}

/* change font for all headings */

h1,
h1 div,
h1 textarea,
.rm-level1 div,
#right-sidebar .rm-level2, /* page headings in right sidebar */
.rm-reference-main .rm-level3 , /* page headings in referenced items */
.rm-level1 textarea,
.roam-log-preview h1,
h1.rm-title-display,
h1.rm-title-display textarea, 
.level1,
.level2 {
  --font-family: "Fira Code", Menlo, monospace;
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  font-weight: 500 !important;
  --letter-spacing: -0.08em;
}

h2,
h2 div,
h2 textarea,
h3,
h3 div,
h3 textarea {
  --font-family: "Fira Code", Menlo, monospace;
  font-family: -apple-system, BlinkMacSystemFont, sans-serif;
  color: #333 !important;
}

/*a {
    color: #106ba3; 
}*/

/* less space below page heading */

.roam-body .roam-app .roam-main .roam-article .rm-title-display {
  margin-bottom: 10px;
}


h1.level2 {
    font-size: 36px !important;
}

/* Main block - remove centering */

.roam-center {
  --align-item: left;
  flex-basis: 40% !important;
}



/* lighter bullets */

#right-sidebar .controls .roam-bullet-closed,
.controls .roam-bullet-closed {
  background: none;
  border: 1px solid silver;
}

.simple-bullet-inner {
  opacity: 0.3;
}

/* lighter vertical guides */

/* Hard to see with the light ones... -Gary
.block-border-left {
  border-color: #eee;
}*/


.roam-block-container h1 {
  font-weight: 300;
  font-size: 26px;
  color: black;
}

.roam-block-container h2 {
  font-weight: 600;
  font-size: 18px;
  color: black;
}

/* align checkboxes better */

label.check-container {
  margin-bottom: 11px;
  margin-right: 3px;
}

/* align checkboxes in zoomed-in headings */

.rm-level1 label.check-container {
  margin-bottom: 17px;
  margin-right: -3px;
}

/* don't shrink block references */

.rm-block-ref {
  font-size: 1em;
  padding: 0;
  margin: 0;
  border-bottom: 0.5px solid #91a8d2; /* darker -Gary */
}

.rm-block-ref label.check-container {
  margin-bottom: 12px;
}

/* wider blocks -Gary */
.rm-block-text {
    max-width: 700px;
}


/* don't need "SHORTCUTS" heading */

.starred-pages-wrapper .flex-h-box {
  display: none;
}

.starred-pages-wrapper > div:first-child {
  margin: 0 -18px;
}

/* more subtle logo */

#roam-sidebar-logo img {
  opacity: 0.4;
}
#roam-sidebar-logo span {
  display: none;
}

/* fade loading astrolabe */

.loading-astrolabe img {
  opacity: 0.2;
}

/* lighter sidebar background */

#right-sidebar {
  background-color: rgba(216, 225, 232, 0.2) !important; 
  /* rgba(216, 225, 232, 0.3) */
  border-left: 1px solid #ddd !important;
}

/* sidebar sections */

#roam-right-sidebar-content > div {
  border-bottom: 1px solid #ddd !important;
  margin: 0 !important;
  padding: 10px 4px 10px 50px;
}

/* sidebar section headings */

#roam-right-sidebar-content > div > div:first-child {
  margin-left: -10px;
}

/* rule under top section of left sidebar */

.roam-sidebar-content > div:first-child {
  padding: 4px 16px !important;
  margin-bottom: 8px;
  border-bottom: 1px solid rgb(57, 75, 89);
}

/* rule under topbar */

.roam-topbar {
  border-bottom: 1px solid #eee;
}

/* crumbs */

.rm-reference-item
  > div:first-child
  > div:first-child
  div
  span:not(.bp3-icon-chevron-right),
.roam-article
  > div:first-child:not(.roam-log-container)
  > div:first-child
  div
  span:not(.bp3-icon-chevron-right) {
  font-size: 12px;
  line-height: 1.3;
  color: #bbb !important;
  /* truncate to smaller width, use css for ellipsis */
  --max-width: 1000px;
  white-space: nowrap;
  overflow: hidden;
  text-overflow: ellipsis;
  padding: 2px !important;
}

.rm-reference-item
  > div:first-child
  > div:first-child
  div
  span:hover:not(.bp3-icon-chevron-right),
.roam-article
  > div:first-child:not(.roam-log-container)
  > div:first-child
  div
  span:hover:not(.bp3-icon-chevron-right) {
  color: black !important;
}

/* chevrons in crumbs */

.roam-reference-item > div > div:first-child .bp3-icon-chevron-right,
.roam-article
  > div
  > div:first-child:not(.roam-log-container)
  .bp3-icon-chevron-right {
  font-size: 1em;
  margin: 0 3px;
  color: #ddd !important;
}

/* no checkboxes in crumbs */

.roam-reference-item
  > div:first-child:not(.roam-log-container)
  > div:first-child
  label.check-container,
.roam-article
  > div:first-child:not(.roam-log-container)
  > div:first-child
  label.check-container {
  display: none;
}

/* link buttons for referenced items */

.rm-reference-main button {
  border: 1px solid #eee;
  border-radius: 0.3em;
  font-size: 0.8em;
}

.rm-reference-main button:hover {
  border-color: #ccc;
}

/* referenced item section headings */

.rm-reference-main {
  --border-top: 1px solid #ededed;
}

.flex-h-box {
    padding-top: 0px !important;
}

.rm-reference-main .flex-h-box {
  min-height: 30px;
}

.rm-reference-main strong {
  color: #222;
  font-size: 0.9em;
  --background-color: rgba(216, 225, 232, 0.3);
}

/* remove background from referenced items */

.rm-reference-item {
  padding: 6px 0 0 0;
  margin: 6px 0 0 0;
  border-top: 1px solid #eee;
  background: none;
}

/* slightly bigger page headings under referenced items */
.rm-reference-main .rm-level3 {
  font-size: 1.6em;
}

/* search */

.rm-find-or-create-wrapper {
  flex: 0 1 100% !important;
}

.rm-find-or-create-wrapper .bp3-input {
  border: none !important;
  box-shadow: none !important;
}

/* highlights */

.roam-highlight {
  --background-color: #c2f9fa;
}

/* links */

a.rm-alias.rm-alias-external {
    color: #b33ba9 !important;
}

a {
    color: #b33ba9;  
}

.rm-page-ref-link-color {
    color: #106ba3;
}

.rm-ref-page-view-title a{
    color: #106ba3;
    font-weight: bold;
}


.level2 a{
    color: #106ba3;
}

/* tweets -- doesn't work */

.twitter-tweet {
    font-size: 7px;
}

/* embeds */

/*.rm-embed-container {
    border: 1px;
    border-color: black;
    border-style: solid;
}*/```
- ### More Colors 
    - Aquae
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FF0gVtucnsb.png?alt=media&token=c192e3a1-3a22-4de6-9f13-9844d349e0b8)
        - Designer::
            - Twitter:: [@calrobert_](https://twitter.com/calrobert_)
            - Love this theme? Say thanks via [Paypal](https://www.paypal.me/calrobertdesign), or donate to Cal's BTC address: 
                - 3Js5L1yhT35dC3jPVj95TQz7gtbD3vE33K
        - Special Features::
            - Inspired by Xcode and Bear
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
/*Add styling with Chrome Stylus Extension
https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne?hl=en
*/

#buffer { /* HIDES BOTTOM RIGHT HELP ICON */
    visibility: hidden;
}

/* ARTICLE WIDTH */

.rm-block-text {
  max-width: 1100px;
}

.roam-article {
    max-width: 1100px;
    padding-left: 20px;
}

.roam-body .roam-app .roam-main .roam-article {
    position: relative;
    padding: 16px 42px 120px;
}

.roam-block-container {
    max-width: 1100px;
}

/* ARTICLE PADDING */

#rm-log-container {
    padding-right: calc((100% - 900px) / 2) !important;
    padding-left: calc((100% - 900px) / 2) !important;
    height: 100% !important;
    overflow: hidden scroll !important;
}

/* Centers text in main article, creates a bug in Graph Overview however, so turning it off
.roam-center > div:nth-child(1) {
    padding-right: calc((100% - 900px) / 2) !important;
    padding-left: calc((100% - 900px) / 2) !important;
    height: 100% !important;
    overflow: hidden scroll !important;
}
*/

/* MAIN DIV ELEMENTS COLORS & BORDERS */
body {
    background-color: #ffffff;
}

.roam-topbar {
    background-color: rgb(250, 252, 253) !important;
    border-bottom: 1px solid #eaeaea;
}

#right-sidebar {
    background-color: rgb(250, 252, 253) !important;
    border-left: 1px solid #eaeaea;
}

.roam-body .roam-app .roam-sidebar-container {
    background-color: #2e3234;

}

.roam-log-container .roam-log-page {
    border-top: 1px solid rgb(225, 225, 225);
}

.rm-reference-item { /* the reference boxes at the bottom */
    background-color: rgb(253, 253, 253);
    border-radius: 6px;
    border: 1px solid #e6e6e68a;
}

/* FONT COLORS */

.rm-level3 {
    font-weight: 400;
    font-size: 1.2em;
    color: #75b5ff;
}

.rm-page-ref-brackets {
    color: #bfbfbf;
}

.roam-app { /* primary text colour */
    color: #282828 !important;
}

.block-highlight-yellow {
    background-color: #d3ffa4;
}

.block-highlight-blue { /* the bright blue highlight color */
    background-color: #d8ecff;
}

.check-container input:checked ~ .checkmark { /* Checked color, might be too light for some people! */
    background-color: #dbdbdb;
    border: none;
}

a {
    color: #0073f9;
    text-decoration: none;
}

a:hover {
    color: #5ca7ff;
    text-decoration: none;
}

/* hashtag */
.rm-page-ref-tag {
    color: rgb(190, 190, 190) !important;
    font-weight: 400;
    background-color: rgba(249, 249, 249, .81);
    border-radius: 10px;
    border: 1px solid #e6e6e682;
    padding: 1px 5px 2px;
}

.rm-page-ref-tag:hover {
    background-color: #dbdbdb;
    text-decoration: none;
}

.controls .simple-bullet-outer .simple-bullet-inner {
    border-radius: 50%;
    width: 5px;
    height: 5px;
    background-color: #0069e3;
}

.roam-bullet-closed { /* expandable bullets */
    background-color: #bcdbff;
}

.block-border-left { /* the tree graphics */
    border-left: 2px solid #e8e8e8;
}

.roam-highlight { /* highlighting */
    background-color: #fff1a4;
    color: #424242;
    border-radius: 0px;
    padding: 5px 5px 4px 5px;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button {
    font-weight: 500;
    color: #717171;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
    color: #717171;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper {
    color: #717171;
}

.rm-page-ref-link-color {
    color: #0073f9d4;
}

code {
    background: #f1f6fb;
    border: 1px solid #d5d8db;
}

.rm-pages-row-highlight {
    background-color: #fbfbfb;
}
.rm-pages-row:first-of-type { /* styles colour of all pages table header */
    background-color: #fff !important;
}
.rm-pages-row:hover {
    background-color: #edf6ffd4;
    color: white;
}

/* KANBAN */
.kanban-board {
    background-color: rgb(250, 252, 253);
    border-radius: 10px;
    border: 1px solid #e6e6e6;
    padding: 12px;
}
.kanban-column {
    background-color: #ecececdb;
    border-radius: 4px;
    margin: 4px 8px 0px 4px;
    padding: 4px;
    min-width: 200px;
}
.kanban-card {
    background-color: white;
    border-radius: 4px;
    border: 1px solid #dbdbdb;
    margin: 6px;
    padding: 8px;
}```
    - Roam Beautified   
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2Fk-lzliCvFi.png?alt=media&token=b29902cc-9057-4b50-a15d-6254ab2f0c8c) 
            - Designer Info:: 
                - Twitter:: [@kanjun](https://twitter.com/kanjun)
                - Love this theme? Say thanks via [Paypal](https://www.paypal.me/kanjunqiu)
            - Special Features::
                - Variation on "[[Leyendecker]]" by [[Maggie Appleton]] 
            - Code::
                - Last updated [[June 4th, 2020]]. You can check [Github](https://github.com/kanjun/roam-beautified) for the latest version. 
                - ```css
.h1,
.h2,
.h3,
.h4,
.h5,
.h6,
h1,
h2,
h3,
h4,
h5,
h6 {
    font-family: 'Inter';
}

div,
textarea {
  font-family: 'SF Pro Display';
  font-size: 100.7%;
  color: #2d3c4e
}

.roam-block-container {
    max-width: 1000px;
}

.rm-query {
    border: 0.5px solid #e4e9ec;
    border-radius: 5px;
    
}

.rm-query .rm-query-title {
    background-color: #f7f8f8;
    padding: 0.8em;
    color: #d1dbe2;
    font-size: 80%;
}

.rm-reference-main.rm-query-content {
    padding: 0.8em;
}

.rm-reference-main .rm-reference-item .rm-block-text {
    font-size: 90%;
}

.rm-ref-page-view-title span {
    font-size: 115%
}

.rm-reference-main .rm-reference-item .controls {
    margin-left: -1em;
}

.rm-ref-page-view {
    padding: 0.4em 0.2em;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
    padding: 6px;
    padding-top: 8px;
    font-size: 110%;
}

div.flex-v-box.starred-pages-wrapper > div.flex-h-box > span {
    font-size: 14px;
    opacity: 80%;
    letter-spacing: 0.0em;
}

div.roam-sidebar-container.noselect > div > div {
    font-size: 14px;
    letter-spacing: 0.03em;
    
}

#block-input {
    background: white;
}

.roam-body #block-input > span > div {
    padding: 6px 24px;
    background: white;
}

span.bp3-icon-small.bp3-icon-star {
    display: none;
    visibility: hidden;
}

#right-sidebar > div {
    background-color: #f7f8fa;
}
.rm-page-ref-brackets {
    display: none;
}
.controls .simple-bullet-outer .simple-bullet-inner {
    background-color: #e5e9f2;
}
.block-border-left {
    border-left: 1px solid #fff;
}
.kanban-board {
    background-color: #fff;
}
.kanban-card {
    background-color: white;
    margin: 8px;
    box-shadow: 0px 1px 2px #9EB3C0;
    padding: 10px;
    border-radius: 2px;
    line-height: 1.3em;
}
.kanban-title {
    text-align: center;
    font-weight: bold;
    padding-top: 6px;
}
.kanban-column {
    background-color: #E4EDF2;
    margin: 0px 4px 0px 4px;
    padding: 4px;
    min-width: 200px;
    border-radius: 3px;
}
.rm-block-ref::before {
    content: '';
    display: inline-block;
    width: 10px;
    border-radius: 40px;
    height: 10px;
    background: #33bdea4d;
    margin-right: 5px;
}
.rm-block-ref {
    border-bottom: none;
    font-size: 1em;
    color: #627a9d;
}
.rm-block-ref:hover {
    background: none;
    cursor: pointer;
}
.checkmark {
    background: #fff;
}
.check-container {
    padding-right: 4px;
}
.check-container input:checked ~ .checkmark {
    background: #33bdea;
}
.check-container input:checked ~ .checkmark:after {
    border-color: #fff;
}
.rm-reference-item {
    margin-top: 8px;
    border-radius: 6px;
    border: 1px solid #e4e9ee;
    margin-right: 8px;
    flex: 1 1 100%;
    word-break: break-word;
    background-color: #f7f9fb;
    padding: 8px;
}

.rm-level2 {
    font-size: 1.5em;
}
.rm-level3 {
    color: #939aae;
    font-weight: 400;
    font-size: 1.3em;
}
.rm-page-ref {
    color: #9aabd0;
}
.rm-page-ref-link-color {
    color: #33bdea;
    font-weight: 600;
}
a {
    color: #ec6f35;
}
.roam-body .roam-app .roam-sidebar-container {
    background-color: #f7f8fa;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page,
.roam-body .roam-app .roam-sidebar-container > * {
    opacity: 80%;
    box-shadow: none;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
    background: white;
    color: black;
    opacity: 100%;
}
#buffer.tall {
    height: calc(100vh - 50px);
}
.check-container {
    padding-right: 4px;
}
span.rm-page-ref {
    border-radius: 2px;
    padding-left: 1px;
    padding-right: 1px;
}
.content span.rm-page-ref {
    padding: 4px 1px 1px;
    /* required for fixing azo */
}
.center-proj {
    text-align: center;
}


span.rm-page-ref[data-tag="Projects"] {
    background: #7172FC;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}

span.rm-page-ref[data-tag="Quick Capture"] {
    color: #db3b8d;
    padding: 3px 4px;
    line-height: 1.4em;
    font-weight: 700;
}
```
    - Roam Blue
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FpEJNUqqrgg.png?alt=media&token=8d4c7904-7e2c-4a5a-bc56-5a6199b120d3)
        - Designer:: [[Mark Robertson]]
            - Twitter:: [@Calhistorian](https://twitter.com/Calhistorian)
            - Love this theme? Say thanks via [Paypal](https://paypal.me/calhistorian)
        - Special Features::
            - {{[[TODO]]}} Item #Area: #Due: #[[Start Date:]] #[[Status:]] #[[Highest Priority]]
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
"/*### ROAM CUSTOM THEME -- Light Mode (Blue)###
*/
/* Editor Style */
/* Sidebar */
/* Left Navigation Pane and Text */
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
background-color: #fff;
color: #0f6ca4;
font-size: 16px;
font-weight: bold;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover {
background-color: #b3d7ff;
color: #3d516d;
border-radius: 15px;
padding-left: 10px;
}
/* Sidebar Hover */
/* Omni Sidebar Hover State */
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
color: #3d516d;
background-color: #b3d7ff;
border-radius: 15px;
}
/* Side Bar Open/Close Icon */
.bp3-button:before,
.bp3-minimal:before,
.bp3-icon-menu:before,
.bp3-small:before {
color: #0d6da5 !important;
}
/* Font */
div {
font-family: 'Futura';
line-height: 1.2em;
margin: 0px;
padding: 0px;
/* font-weight: bold; */
}
.roam-body .roam-app .roam-main .roam-article {
color: #444444;
}
/* Header Styles */
.roam-app h1 {
/* styles page titling */
color: #3d516d !important;
font-weight: bold;
}
.roam-app h2 {
/* styles page titling */
color: #3d516d !important;
font-weight: bold;
}
.roam-app h3 {
/* styles page titling */
color: #3d516d !important;
font-weight: bold;
}
/* Selection Style */
.rm-block-input {
background-color: #b3d7ff;
border-radius: 10px;
padding-left: 5px;
padding-right: 5px;
}
.block-border-left {
/* the tree/outline graphics */
border-left: 1px solid #b3d7ff;
}
/* Bullets */
.controls .simple-bullet-outer .simple-bullet-inner {
border-radius: 50%;
width: 5px;
height: 5px;
background-color: #009aff;
}
/* bullet indent width */
.flex-v-box {
margin-left: 13px !important;
}
/* expandable bullets */
.roam-bullet-closed {
background-color: #b3d7ff;
}
/* Top and Bottom Bars in Nav Bar */
.roam-body .roam-app .roam-sidebar-container {
background-color: #fff;
}
/* Roam Search Box */
.bp3-input,
.bp3-input[readonly] {
background: #edf5ff;
box-shadow: inset 0 0 0 1px #337ab7;
}
/* Text in Search Results Box */
.rm-find-or-create-wrapper .rm-menu-item .rm-search-list-item {
word-break: break-word;
color: black;
overflow-wrap: break-spaces;
margin-left: -20px;
}
/* New Page Style */
.rm-find-or-create-wrapper .rm-menu-item .rm-search-title .rm-new-page {
color: #e7424e;
}
/* Popup Style */
.bp3-popover-content {
background: white !important;
}
.bp3-popover .bp3-popover-arrow-fill {
fill: #337ab7;
}
.bp3-popover .bp3-popover-content,
.bp3-menu {
background: #ffffff !important;
color: #3d516d;
box-shadow: 0 0 0 1px rgba(14, 83, 152, .76), 0 2px 4px rgba(20, 73, 127, .81)/*,
/*0 8px 24px rgba(16, 22, 26, 0.2)*/;
}
/* Slash Popup */
.bp3-elevation-3 {
color: black;
background-color: #b0d4fc;
border-radius: 4px;
box-shadow: 0 0 0 1px rgba(14, 83, 152, .76), 0 2px 10px rgba(20, 73, 127, .81)/*,
/*0 8px 24px rgba(16, 22, 26, 0.2)*/;
}
/* Block Reference Style */
.rm-block-ref {
padding: 4px 2px;
margin: -4px 0px;
font-size: 12px;
display: inline;
border-bottom: 1px solid #0d6da5;
cursor: alias;
padding-left: 0px;
/* RTB add: align to left */
}
.rm-block-ref:hover {
background-color: #b3d7ff;
border-radius: 8px;
}
/* Reference Separator */
.rm-reference-container {
border-top: 3px solid #202b33;
padding-top: 12px;
margin-bottom: 8px;
}
/* the reference boxes at the bottom */
.rm-reference-item {
background-color: #e7f2ff;
border-radius: 10px;
padding-left: 20px;
}
/* Reference Titles */
.roam-article > div:last-child a {
color: #029aff !important;
font-weight: bold;
/*padding-left: 20px !important;*/
}
/* Kanban Style */
.kanban-board {
background-color: #fff;
}
.kanban-card {
background-color: white;
margin: 8px;
box-shadow: 0px 1px 2px #9EB3C0;
padding: 10px;
border-radius: 2px;
line-height: 1.3em;
}
.kanban-title {
text-align: center;
font-weight: bold;
padding-top: 6px;
}
.kanban-column {
background-color: #E4EDF2;
margin: 0px 4px 0px 4px;
padding: 4px;
min-width: 200px;
border-radius: 3px;
}
/* Roam Page Sorter */
.rm-pages-row .rm-pages-col {
color: black;
padding: 8px 4px;
flex: 1 0 15%;
}
/* Text Styles */
.roam-highlight {
background-color: #f8ee4d;
margin: -2px;
padding: 2px;
}
/* Namespace Color */
.rm-page-ref-namespace-color {
color: green;
}
.check-container {
display: inline-block;
position: relative;
padding-left: 20px;
/* RTB change: align checkbox for updated spacing */
margin-bottom: 7.5px;
cursor: pointer;
font-size: 48px;
-webkit-user-select: none;
-moz-user-select: none;
-ms-user-select: none;
user-select: none;
vertical-align: bottom;
top: -12px;
/* RTB change: align checkbox for updated spacing */
}
/* Hide the browser's default checkbox */
.check-container input {
position: absolute;
opacity: 0;
cursor: pointer;
height: 0;
width: 0;
}
/* Create a custom checkbox */
.checkmark {
position: absolute;
top: -3px;
left: 0px;
height: 18px;
border-radius: 10px;
width: 18px;
border: 2px solid #009aff;
}
/* On mouse-over, add a grey background color */
/* When the checkbox is checked, add a background coloor */
.check-container input:checked ~ .checkmark {
background-color: #009aff;
/* purple theme color */
border: none;
}
/* Create the checkmark/indicator (hidden when not checked) */
.checkmark:after {
content: "";
position: absolute;
display: none;
padding-left: 2px;
}
/* Show the checkmark when checked */
.check-container input:checked ~ .checkmark:after {
display: block;
}
/* Style the checkmark/indicator */
.check-container .checkmark:after {
left: 4.9px;
top: 2px;
width: 7px;
height: 11px;
border: solid white;
border-width: 0 3px 2.5px 0;
-webkit-transform: rotate(45deg);
-ms-transform: rotate(45deg);
transform: rotate(40deg) scale(1);
}```
            - Tag styles
                - ```css
"
.rm-page-ref-tag {
color: #617a99 !important;
background-color: #ecf5ff;
border-radius: 8px;
padding: .5px 3.5px .5px 3.5px;
}
.rm-page-ref-tag:hover {
color: #202b33 !important;
background-color: #b3d7ff;
text-decoration: none;
}
span.rm-page-ref[data-tag=\"Area:\"] {
background-color: #b3e1ff !important;
font-size: 12px;
color: black !important;
letter-spacing: .07em;
padding: 0px 3px 0px 3px;
}
span.rm-page-ref[data-tag=\"Area:\"]::before {
content: " "
}
span.rm-page-ref[data-tag=\"Due:\"] {
background-color: #b3e1ff !important;
font-size: 12px;
color: black !important;
letter-spacing: .07em;
padding: 0px 3px 0px 3px;
}
span.rm-page-ref[data-tag=\"Due:\"]::before {
content: " "
}
span.rm-page-ref[data-tag=\"Start Date:\"] {
background-color: #b3e1ff !important;
font-size: 12px;
color: black !important;
letter-spacing: .07em;
padding: 0px 3px 0px 3px;
}
span.rm-page-ref[data-tag=\"Start Date:\"]::before {
content: " "
}
span.rm-page-ref[data-tag=\"Status:\"] {
background-color: #b3e1ff !important;
font-size: 12px;
color: black !important;
letter-spacing: .07em;
padding: 0px 3px 0px 3px;
}
span.rm-page-ref[data-tag=\"Status:\"]::before {
content: " "
}
span.rm-page-ref[data-tag=\"Subtasks:\"] {
background-color: #e6d35c !important;
color: black !important;
letter-spacing: .07em;
padding: 0px 3px 0px 3px;
}
span.rm-page-ref[data-tag=\"Subtasks:\"]::after {
content: " ✔"
}```
    - Roamness
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FfvvyJsdyjl.png?alt=media&token=d90bcad3-e7eb-44a3-8a4d-e67c2023949a)
        - Designer:: [[Anne-Laure Le Cunff]]
            - Twitter:: [@anthilemoon](https://twitter.com/anthilemoon) 
            - Love this theme? Say thanks via [Paypal](https://www.paypal.me/alecunff)
        - Special Features::  
        - Code::
            - Last updated [[June 4th, 2020]]
            - ```css
/* Roamness theme for Roam Research by Ness Labs: https://nesslabs.com/ */

body {
background-color: #ffffff;
}

.roam-topbar {
background-color: #121212;
}

input#find-or-create-input:focus {
box-shadow: 0 0 0 1px #16b7b7;
}

span.bp3-icon-small.bp3-icon-star {
display: none;
visibility: hidden;
}

.roam-body .roam-app h1 {
color: #121212;
font-family: 'Georgia';
}

div,
textarea {
font-family: 'Georgia';
font-size: 16px;
color: #121212
}

.roam-highlight {
background-color: #c4edf1;

}

#right-sidebar > div {
background-color: #faffff;
border-left: 1px solid #e5e5e5;
}

.roam-body .roam-app .roam-sidebar-container {
background-color: #faffff;
border-right: 1px #e5e5e5 solid;
}
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page,
.roam-body .roam-app .roam-sidebar-container > * {
background-color: #faffff;
color: #121212;
box-shadow: none;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover {
background-color: #faffff;
color: #048a8a;
}

a {
color: #16b7b7;
}

a:hover {
color: #048a8a;
text-decoration: none;
}

strong {
color: #0a4747;
}

em {
color: #0a4747;
}

.cm-s-default .cm-keyword {
color: #048a8a;
}

.checkmark {
background: #ffffff;
}

.check-container input:checked ~ .checkmark {
background: #16b7b7;
}

.check-container input:checked ~ .checkmark:after {
border-color: #ffffff;
}

.rm-query {
border: 0.5px solid #048a8a;
border-radius: 5px;
}

.rm-query .rm-query-title {
background-color: #ffffff;
color: #121212;
}

.rm-reference-main .rm-reference-item .rm-block-text {
font-size: 90%;
}

.rm-ref-page-view-title span {
color: #121212;
text-decoration: none;
}

#block-input {
background: #ffffff;
}

.roam-body #block-input > span > div {
background: #ffffff;
}

.controls .simple-bullet-outer .simple-bullet-inner {
background-color: #0a4747;
}

.block-border-left {
border-left: 1px solid #ffffff;
}

.rm-reference-item {
margin: 10px 10px 10px 0px;
padding: 8px;
border-radius: 3px;
border: 1px solid #e5e5e5;
word-break: break-all;
background-color: #faffff;
}

.rm-level3 {
color: #121212;
}

.rm-page-ref {
color: #121212;
}

.rm-page-ref-link-color {
color: #16b7b7;
}

.rm-title-textarea {
font-size: 36px;
}

span.rm-page-ref[data-tag="to read"] {
color: #ffffff;
background-color: #16b7b7;
border: 1px #ffffff;
border-radius: 3px;
padding: 3px 6px;
}

span.rm-page-ref[data-link-title="to process"] {
color: #ffffff;
background-color: #16b7b7;
border: 1px #ffffff;
border-radius: 3px;
padding: 3px 6px;
}

span.rm-page-ref[data-tag="to process"] {
color: #ffffff;
background-color: #048a8a;
border: 1px #ffffff;
border-radius: 3px;
padding: 3px 6px;
}

span.rm-page-ref[data-tag="to write"] {
color: #ffffff;
background-color: #0a4747;
border: 1px #ffffff;
border-radius: 3px;
padding: 3px 6px;
}```
    - Slightly Aesthetic 
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FVVu_LnA6Y0.png?alt=media&token=be40ffe9-7889-4ff5-afac-924445ceef26)
        - Designer::
            - Twitter:: [@al_malecha](https://twitter.com/al_malecha) 
            - Love this theme? Say thanks via [Paypal](https://www.paypal.me/almalecha)
        - Code::
            - Last updated [[June 4th, 2020]]. You can check [Github](https://github.com/allymalecha/slightly-aesthetic-roam-theme) for the latest version. 
            - ```css
"/* Slighly aesthetic roam theme with teal, lavender, gray, and a fun load screen
By Al but with a lot of help from smart individuals on Reddit
V 1.0
*/

@import url('https://fonts.googleapis.com/css?family=Work+Sans&display=swap');

/* General formatting of the site */
/* Make page width wider */
.roam-block-container,.roam-block,.rm-block-text {max-width: 900px;}

.roam-center > div {padding-right: 20px !important;padding-left: 20px !important;}
/* end page widening */

body { /*    Background color   */
    background-color: #E2E2E2;
}

div { 
    font-family: 'Work Sans', serif;
}

.level2 {
    font-family: 'Work Sans', serif;
}

/* Header bar */
.roam-topbar { 
    background-color: #CECBDB;
}


/* Left side bar style*/
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper,
.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page {
        background-color: #2C4251;
    color: #CECBDB;
  font-size: 16px;
}

/* Change sideboard to all one color */
.roam-body .roam-app .roam-sidebar-container {
background-color: #2C4251 !important;
}

/* Change color of the email address in upper left */
.bp3-button div {
color: #58A4B0 !important;
}

/* Left side Bar Open/Close Icon and star/calendar icons in header */
.bp3-icon-star-empty::before {
    content: "🌟";
}

.bp3-icon-graph:before,
.bp3-icon-star:before,
.bp3-icon-star-empty:before,
.bp3-icon-more:before,
.bp3-icon-menu:before,
.bp3-button:before, 
.bp3-minimal:before, 
.bp3-small:before, 
.bp3-icon-filter {
  color: #58A4B0 !important;
}
/* Left side Bar Hovering */

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .starred-pages-wrapper .starred-pages .page:hover {
  color: black;
  background-color: #58A4B0;
}

.roam-body .roam-app .roam-sidebar-container .roam-sidebar-content .log-button:hover { 
  color: black;
  background-color: #58A4B0;
}

/*Change Roam Research logo color to match theme*/
#roam-sidebar-logo {
    color:#CECBDB
}
        
/*/ Roam Search Bar /*/

/* Roam Search Box Placeholder Text Color */
.bp3-input::placeholder,
.bp3-input-group > .bp3-icon {
    color: #58A4B0;
}

/* Input Text Color in Search Bar */
.bp3-input {
  color: black;
}

/* New Page Button Color */
.rm-find-or-create-wrapper .rm-menu-item .rm-search-title .rm-new-page {
  color: #58A4B0;
}

.bp3-button .bp3-minimal .bp3-intent-success {
    color: #58A4B0   
}

.bp3-button .bp3-minimal .bp3-intent-success a:hover {
    background-color: #CECBDB;   
}

/* Body */

/* tree style */
.block-border-left { 
    border-left: 2px solid #58A4B0;
}

/* Bullets */
.controls .simple-bullet-outer .simple-bullet-inner {
  border-radius: 50%;
  width: 5px;
  height: 5px;
  background-color: #58A4B0; 
}
.roam-bullet-closed { 
    background-color:  #CECBDB;
}

/* Markdown link titles */

.roam-app a {
  color: #58A4B0;
}

.roam-app a:focus, 
.roam-app a:hover {
  color: #58A4B0;
  text-decoration: underline;
}

/* external link color */
a.rm-alias.rm-alias-external {
    color: #106ba3 !important;
}

/* the currently selected block */
 .rm-block-input{ 
  color: #2C4251 !important;
    font-family: 'Work Sans', serif;
     background-color:  #CECBDB;
     } 


/* Tagging style */
.rm-page-ref-tag { /* hashtags */
    color: #EBFAFF !important;
    background-color: #58A4B0;
    border-radius: 10px;
    padding: 2px 3px 2px 3px;
}

/* external link color */

a.rm-alias.rm-alias-external {
    color: #58A4B0 !important;
}

/* Header Styles */

.roam-app h1 { /* styles page titling */
    color: #2C4251 !important;
    font-weight: bold;
  font-size: 36px;
  
}
.roam-app h2 { /* styles page titling */
    color: #2C4251 !important;
    font-weight: bold;
  font-size: 32px;
}
 .roam-app h3 { /* styles page titling */
    color: #2C4251 !important;
    font-weight: bold;
  font-size: 24px;
}
.roam-app h4 { /* styles page titling */
    color: #2C4251 !important;
    font-weight: bold;
  font-size: 18px;   
}

/* Reference Titles */
.roam-article > div:last-child a { 
    color: #2C4251 !important;
}

/* Reference Boxes */
.rm-reference-item { 
  background-color: #EBFAFF;
    border-radius: 15px;
    padding: 20px;
}

/* Right side bar color */
#right-sidebar {
    background-color: #EBFAFF !important;
}


/* Right side bar reference boxes */
#right-sidebar .rm-reference-item { 
  background-color: #E2E2E2;
    border-radius: 15px;
    padding: 20px;
}

/*Wraps text when I'm doing an inline search with [[]] or (())*/
.bp3-text-overflow-ellipsis {
    text-overflow: unset;
    white-space: unset;
}
/* hover color in search bar*/
.rm-mentions-search-items .rm-mentions-search-item:hover {
  background-color: #bfccd6;
}
/* wrap overflow text in dropdown menu */
.bp3-text-overflow-ellipsis {
    text-overflow: unset;
    white-space: unset;
}

/* reference main */
.roam-block .rm-reference-main {
    padding: 0px 16px 12px 16px;
    background-color: whitesmoke;
    border-radius: 15px;
}

/* nicer looking block quote */
:root {
  --blockquote-font-color: rgba(109, 156, 190, 0.89);
  --blockquote-border-color: #444;
  --blockquote-bg: none;
  --blockquote-cite: #777;
}

/* change highlight color, general text highlighting and block highlighting */

.roam-highlight {
        background-color: #AEFFEA;
    }
 .block-highlight-blue {
            background-color: white;
        }
/* change loading bar to something that doesn't make me aggravated */

.loading-astrolabe{
	display: block;
 	-moz-box-sizing: border-box;
  	box-sizing: border-box;
 	background: url(https://i.imgur.com/KWl6pqT.gif) no-repeat;
  	width: 600px;
  	height: 600px;
  	padding-left: 600px; /* Equal to width of new image */
}
.loading-astrolabe .wand{
	visibility: hidden;
}
/* path view tags at top same color as rest of background */
.zoom-path-view .rm-zoom-mask {
    mix-blend-mode: saturation;
    background-color: #E2E2E2;
    flex: 1 1 100%;
}
/* block reference background color */
.rm-block-ref {
    background-color:#CECBDB;
}
/* tag colors, add your own in data-tag to change colors */
span.rm-page-ref[data-tag="question"] {
    background: #7172FC;
    color: #fff;
}
span.rm-page-ref[data-tag="factcheck"] {
    background: #21897E;
    color: #fff;
}```
    - [[Yggdrasil]]
        - ![](https://firebasestorage.googleapis.com/v0/b/firescript-577a2.appspot.com/o/imgs%2Fapp%2Froam%2FT0iQmFOXwm.png?alt=media&token=3cdca40f-d2bb-4217-9f26-b44c825f88be)
        - Designer:: [[Azlen Elza]]
            - "Twitter:: [@azlenelza](https://twitter.com/azlenelza) "
            - "Love this theme? Say thanks via [Paypal](https://www.paypal.me/azlenelza). "
            - Also created "[[Cosmonaut]]" and "[[Zenith]]"
        - Special Features:: 
            - "Collapsible columns -- side-by-side view for items opened in the sidebar "
            - "Searchbar appears in main page "
            - "Overlay side-by-side view over graph/diagram"
        - Code::
            - ```css
/* IMPORT CORE THEME */
@import url('https://azlen.github.io/roam-themes/core.css');

/* GOOGLE FONTS */
@import url('https://fonts.googleapis.com/css2?family=Crimson+Text:ital,wght@0,400;0,700;1,400;1,700&display=swap');

/* VARIABLES */
:root {
    --page-width: 616px;
    
    --header-font: "Crimson Text", serif;
    --body-font: "Crimson Text", serif;
    
    --bg-color: #f5f1e2;
    --page-color: rgba(236, 231, 209, .95);
    
    --text-color: #000000;
    --icon-color: #5c7080;
    --bullet-color: rgba(0, 0, 0, 0.2);
    
    --page-shadow: 0px 8px 14px rgba(0, 0, 0, 0.02);
    --color-primary: 181, 124, 38;
    --color-primary-contrast: #FFFFFF;
    --color-secondary: 100, 181, 38;
    
    --color-secondary-contrast: #FFFFFF;
}

/* YGGDRASIL CUSTOM STYLES */

.rm-page-ref-tag {
    padding: 3px 6px 2px 6px;
}

/* reverse colours for saving / saving-remote so that green is used for "saved" */
.rm-saving-icon .rm-synced {
    background-color: rgb(var(--color-secondary));
}
.rm-saving-icon .rm-saving-remote {
    background-color: rgb(var(--color-primary));
}

.block-bullet-view .bp3-button:not([class*="bp3-icon"]) {
    padding: 5px 14px 0px 14px!important;
}

.kanban-card {
    box-shadow: 0px 1px 2px rgba(0,0,0, 0.3);
}
.kanban-column {
    background-color: var(--bg-color);
}

/* CHANGE COLOURS IN CANVAS */

canvas[data-id="layer2-node"] {
    filter: invert(1) hue-rotate(170deg) saturate(2.5);
}```
- ### Block Level Customizations
    - [[roam/css]]
    - from [[Maggie Appleton]] in "[[Leyendecker]]"
        - {{[[embed]]: ((HdHehJEXV))}}
