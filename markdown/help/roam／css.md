- [[Conor]]
    - ```css
.group {
  display: flex;
  align-items: center;
  flex-direction: row;
}
.group div {
  border: none;
}
.group > .rm-block__self {
  flex-grow: 0.1;
}
.group .rm-block__children .rm-block__controls {
opacity: 0;
}
.group:hover .rm-block__children .rm-block__controls {
opacity: 1;
}

.group > .rm-block__children {
   flex-grow: 1;
  margin: 12px 4px;
  padding: 8px 0px;
  border-top: 1px solid green;
  border-bottom: 1px solid green;
  border-left: 1px solid green;
}```
    - ```css
.grey-hl .rm-highlight {
  background-color: transparent;
  color: gray;
}
```
    - ```css
.big .rm-highlight {
  background-color: transparent;
  font-size: 2em;
}```
    - ```css
.Falsified {
text-decoration: line-through;
}```
    - Old Block level styling
        - ```css
.roam-block-container[data-page-links*="horizontal"] 
.rm-block-children {
  display: flex;
  flex-direction: row;
 
}
.roam-block-container[data-page-links*="horizontal"] 
 .rm-block__controls {
  display: none;
 
}```
        - Hide the tag
            - ```css
span.rm-page-ref[data-tag="rm-h"] {
    display: none;
}

.roam-block-container[data-page-links*="rm-h"] .rm-block-children {
  display: flex;
  flex-direction: row;
}
```
        - Grid `#rm-grid`
            - ```css

.roam-block-container[data-page-links*="rm-grid"] .rm-block-children {
  display: grid;
  background-color: #F7F8F8;
  
 grid-template-columns: repeat( auto-fit, minmax(150px, 1fr) );
}```
        - Blue border for children
            - ```css
.rm-block[data-path-page-links*="rm-blue-border--children"]{
  border: 1px solid blue;
}```
        - Span 2 columns
            - ```css
.roam-block-container[data-page-links*="rm-col-span2"] {
  grid-column: span 2;
}```
        - Span 2 rows 
            - ```css
.roam-block-container[data-page-links*="rm-row-span2"] {
  grid-row: span 2;
}```
        - Hide the `.rm` tags
            - ```css
.roam-block-container[data-page-links*="rm-hide"]
span.rm-page-ref[data-tag*="rm"] 
{
  display: none;
}```
    - New block level styling
        - ```css
.bblue {
  border: 2px solid blue !important;
}```
        - ```css
.green  {
  margin: 2px;
  background-color: green;
  color: white;
}```
- #Evergreens
- Live Editor for playing with custom tags {{[[table]]}}
    - ```css

span.rm-page-ref[data-tag="Evergreens"] {
    background: #FF5722 !important;
    color: #fff !important;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
}
```
        - #Evergreens
    - ```css
span.rm-page-ref[data-tag="Seedling"] {
    color: #4CAF50 !important;
    padding: 3px 3px;
    font-weight: 600;
    line-height: 1.4em;
}
```
        - #Seedling 
    - ```css
span.rm-page-ref[data-tag="Idea Bank"] {
    color: #3C34EA !important;
    padding: 3px 4px;
    font-weight: 700;
    line-height: 1.4em;
}

span.rm-page-ref[data-tag="Idea Bank"]:before {
    content: '✦ '
}
```
        -  #[[Idea Bank]]
    - ```css
span.rm-page-ref[data-tag="Essay"] {
    background: #03A9F4;
    color: #fff;
    padding: 3px 7px;
    line-height: 2em;
    font-weight: 500;
}
```
        - #Essay
- Make wide
    - ```css
[data-tag="make:wide"] ~ div {
	width: 110% !important;
}

[data-tag="make:wide-x"] ~ div {
	width: 120% !important;	
}

[data-tag="make:wide-xx"] ~ div {
	width: 130% !important;	
}

[data-tag="make:wide-xxl"] ~ div {
	width: 150% !important;
}


[data-tag="make:wide-on-hover"] ~ div:hover {
  transform: scale(1.5); 
}

[data-tag*="make:wide"] ~ div div:nth-child(2){
	width: 100% !important;
}



[data-tag="make:long"] ~ div {
	height: 660px !important;
}

[data-tag="make:long-x"] ~ div {
	height: 760px !important;
}

[data-tag="make:long-xx"] ~ div {
	height: 860px !important;
}

[data-tag="make:long-xxl"] ~ div {
	height: 960px !important;
}


[data-tag*="make:long"] ~ div div:nth-child(2){
	height: 100% !important;
}```
- Customizing Nested Tables and embeds
    - ```css
/* don't limit the block width for tables */
span.rm-page-ref[data-tag="make:table-tight"] ~ div .rm-block-text {
    max-width: none!important;
}

/* clean up tables embedded in tables and blocks within tables */
span.rm-page-ref[data-tag="make:table-tight"] ~ div .roam-table, .roam-table th, .roam-table td, .roam-table tr {
    padding:0!important;
    vertical-align: top;
    min-width:auto!important;
    overflow: hidden;
}

span.rm-page-ref[data-tag="make:table-tight"] ~ div .roam-table .roam-table table {
    width:100%;
}

span.rm-page-ref[data-tag="make:table-tight"] ~ div .roam-table .rm-block-ref {
    padding:0!important;
}

span.rm-page-ref[data-tag="make:table-tight"] ~ div .roam-table .rm-embed-container {
    background-color:transparent!important;
    padding-bottom:20px;
}

span.rm-page-ref[data-tag="make:table-tight"] ~ div .roam-table .rm-embed-edit, .roam-table .bp3-popover-wrapper {
    display:none!important;
}

span.rm-page-ref[data-tag="make:table-tight"] ~ div .roam-table .controls .block-expand .rm-caret {
    transition:none!important;
}

span.rm-page-ref[data-tag="make:table-tight"] ~ div .rm-embed-inner-block-hide:hover {
    margin-left:-42px!important;
}

span.rm-page-ref[data-tag="make:table-tight"] ~ div .roam-table .roam-table th, .roam-table  .roam-table td, .roam-table  .roam-table tr {
    border-bottom:0;
    border-left:0;
    border-top:0;
}

```
