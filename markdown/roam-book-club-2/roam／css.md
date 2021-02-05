- see also: [[roam/js]]
    - (last updated 08:17 PST Wednesday [[November 5th, 2020]] by [[Matt Brockwell/MJB]])
- (CSS mods to this database are indented below, to allow us to "view as numbered list")
    1. This one makes block references more visible:

        - The purpose of this is to allow in-line commenting on other people's comments to more clearly show visually which part is a "quote" that we are responding to, and which part is the "new speaker" speaking.

            - also note that, since this now provides a strong visual cue that something is a block, I'm taken the liberty of turning off the underlining as well, because it now seems redundant. 
        - CSS below:
            - ```css
/* turn off underlining */ 
.rm-block-ref{
    border-bottom: none;
}

/* recolor the block reference */

.rm-block-ref{
    background-color: #ffffe3;
}```
    2. Here's a special CSS for # `sub`:
        - ```css
span.rm-page-ref[data-tag="sub"]:before {
    content: "🔽 "
}

span.rm-page-ref[data-tag="sub"] {
    background: #BB8B4063 !important;
    color:  #3B0248 !important;
    padding: 2px 5px;
    line-height: 2em;
    font-weight: 500;
}```
    3. Here's a special CSS for # `deepdive` :
        - ```css
span.rm-page-ref[data-tag="deepdive"]:before {
    content: "🤿 "
}

span.rm-page-ref[data-tag="deepdive"] {
    background: #10027363 !important;
    color:  #E7FCFF !important;
    padding: 2px 5px;
    line-height: 2em;
    font-weight: 500;
}```
    4. Special CSS use-case where implementing `Fleeting`, `Branching`, `Intermediary` and `Permanent` Notes are colored with a gradient (Aesthetically pleasing 🎨) (from [[Beau Haan 📌]])
        - #[[Fleeting Notes]] [[Test]]
            - ```css
span.rm-page-ref[data-tag="Fleeting Notes"] {
	background: #fff;
	background-size: 100%;
    color: #000;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
   border-style: solid;
  border-color: #f21da140;
  border-width: thin;
    position:relative;
  
    
  box-shadow: 0px 1px 3px -1px #000000, 
            0px -1px 5px  #DFDFDF;
  
  
}








```
                - ```css
span.rm-page-ref[data-tag="Fleeting Notes"] {
    color: #1A1718 !important;
    padding: 2px 5px 2px 5px;
	font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FFEFBA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FFFFFF, #FFEFBA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #FFFFFF, #FFEFBA); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}




```
        - #[[Literature Notes]] [[Test]]
            - ```css
span.rm-page-ref[data-tag="Literature Notes"] {
background: #fff;
	background-size: 100%;
    color: #000;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
   border-style: solid;
  border-color: #215F0040;
  border-width: thin;
    position:relative;
    
  box-shadow: 0px 1px 3px -1px #000000, 
            0px -1px 5px  #DFDFDF;
}








```
        -  #[[Fleeting Notes]] updated
            - ```css
span.rm-page-ref[data-tag="Fleeting Notes"] {
	background: #fff;
	background-size: 100%;
    color: #000;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
   border-style: solid;
  border-color: #FFEFBA;
  border-width: thin;
    position:relative;
}

 span.rm-page-ref[data-tag="Fleeting Notes"] + span[data-link-title] {
     background: #fff !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 5px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0px 5px 5px 0px;
     margin-left: -5px;
}






```
        - #[[Reference Notes]] [[Test]]
            - ```css
span.rm-page-ref[data-tag="Reference Notes"] {
background: #fff;
	background-size: 100%;
    color: #000;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
   border-style: solid;
  border-color: #f26e1d40;
  border-width: thin;
    position:relative;
  
    
  box-shadow: 0px 1px 3px -1px #000000, 
            0px -1px 5px  #DFDFDF;
  
  
}

```
        - #Zettels [[Test]]
            - ```css
span.rm-page-ref[data-tag="Zettels"] {
	background-image: linear-gradient(90deg, #1DA1F2, #1DA1F2);
	background-size: 100%;
    color: #FFFFFF;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 3px 0 0 3px;
    position:relative;
  
    box-shadow: 0px 1px 3px -1px #000000, 
            0px -1px 5px  #DFDFDF;
}

 span.rm-page-ref[data-tag="Zettels"] + span[data-link-title] {
     background: #1DA1F21E !important;
     color: #F5F8FA !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
   

}


span.rm-page-ref[data-tag="Zettels"]:after, span.rm-page-ref[data-tag="Zettels"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;

}

span.rm-page-ref[data-tag="Zettels"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #1DA1F2;
    border-width: 10px;
    margin-top: -10px;

}

span.rm-page-ref[data-tag="Zettels"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #1DA1F2;
    border-width: 10px;
    margin-top: -10px;

}





```
        - #[[Literature Notes]] [[Test]] updated
            - ```css
span.rm-page-ref[data-tag="Literature Notes"] {
background: #fff;
	background-size: 100%;
    color: #000;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
   border-style: solid;
  border-color: #215F0040;
  border-width: thin;
    position:relative;
}

 span.rm-page-ref[data-tag="Literature Notes"] + span[data-link-title] {
     background: #F5F8FA !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 5px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0px 5px 5px 0px;
     margin-left: -5px;
}






```
        - #[[Relevant Notes]] [[Test]]
            - ```css
span.rm-page-ref[data-tag="Relevant Notes"] {
background: white;
	background-size: 100%;
    color: #1DA1F2;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
   border-style: solid;
  border-color: #FFFFFF;
  border-width: thin;
    position:relative;
  
  box-shadow: 0px 1px 3px -1px #000000, 
            0px -1px 5px  #DFDFDF;
  
  
}

 span.rm-page-ref[data-tag="Relevant Notes"] + span[data-link-title] {
     background: #1DA1F210 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 8px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0px 5px 5px 0px;
     margin-left: -8px;
   
   
box-shadow: inset -1px 1px 5px #AAAAAA63, 
            inset 1px -1px 3px #F6F6F6;
   
}

```
        - #[[Branching Notes]] [[Test]]
            - ```css
span.rm-page-ref[data-tag="Branching Notes"] {
background: #B79891;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #94716B, #B79891);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #94716B, #B79891); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */

	background-size: 100%;
    color: #EEF2EE;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
    position:relative;
}

 span.rm-page-ref[data-tag="Branching Notes"] + span[data-link-title] {
     background: #B7989128 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 5px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0px 5px 5px 0px;
     margin-left: -5px;
}





```
        - #[[Relevant Notes]] [[Test]]
            - ```css
span.rm-page-ref[data-tag="Relevant Notes"] {
background: white;
	background-size: 100%;
    color: #1DA1F2;
    padding: 2px 5px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 5px 5px 5px 5px;
   border-style: solid;
  border-color: #FFFFFF;
  border-width: thin;
    position:relative;
  
  box-shadow: 0px 1px 3px -1px #000000, 
            0px -1px 5px  #DFDFDF;
  
  
}

 span.rm-page-ref[data-tag="Relevant Notes"] + span[data-link-title] {
     background: #1DA1F210 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 8px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0px 5px 5px 0px;
     margin-left: -8px;
   
   
box-shadow: inset -1px 1px 5px #AAAAAA63, 
            inset 1px -1px 3px #F6F6F6;
   
}

```
        - #[[Permanent Notes]] [[Test]]
            - ```css
span.rm-page-ref[data-tag="Permanent Notes"] {
	background-image: linear-gradient(90deg, #507B58, #96B09B, #507B58);
	background-size: 100%;
    color: #EEF2EE;
    padding: 2px 2px 2px 5px;
    font-size: 13px;
    line-height: 1em;
    font-weight: 500;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Permanent Notes"] + span[data-link-title] {
     background: #DCE5DE8C !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Permanent Notes"]:after, span.rm-page-ref[data-tag="Permanent Notes"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Permanent Notes"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #507B58;
    border-width: 10px;
    margin-top: -10px;
}

span.rm-page-ref[data-tag="Permanent Notes"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #507B58;
    border-width: 10px;
    margin-top: -10px;
}



```
        - #quote
            - ```css
span.rm-page-ref[data-tag="quote"] {
    background: #A7E2EA !important;
    color: rgb(50,68,213) !important;
    padding: 1px 5px;
    line-height: 2em;
  	border-radius: 4px 4px 4px 20px;
}


span.rm-page-ref[data-tag="quote"]:before {
    content: '✦'
}
```
        10. CSS code for helping make the [[Daily Notes]] page a little more aesthetically pleasing! (from [[Beau Haan 📌]])
            - #Post [[Your Name]]
                - ```css
span.rm-page-ref[data-tag="Post"] {
	background-image: linear-gradient(to right, #607D8B,#607D8B);
	background-size: 100%;
    color: rgb(255,255,255);
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Post"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Post"]:after, span.rm-page-ref[data-tag="Post"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Post"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #607D8B;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Post"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #607D8B;
    border-width: 11px;
    margin-top: -11px;
}

```
            - #Chat [[Your Name]] #@ [[Beau Haan 📌]]
                - ```css
span.rm-page-ref[data-tag="Chat"] {
	background-image: linear-gradient(to right, #4c8dc9,#4c8dc9);
	background-size: 100%;
    color: #EEF2EE;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Chat"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Chat"]:after, 
span.rm-page-ref[data-tag="Chat"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Chat"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Chat"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}
```
            - #Reply [[Your Name]]
                - ```css
span.rm-page-ref[data-tag="Reply"] {
	background-image: linear-gradient(to right, #E5E5EA,#E5E5EA);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Reply"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Reply"]:after, span.rm-page-ref[data-tag="Reply"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Reply"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #E5E5EA;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Reply"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #E5E5EA;
    border-width: 11px;
    margin-top: -11px;
}

```
            - #Question [[Their Name]]
                - ```css
span.rm-page-ref[data-tag="Question"] {
	background-image: linear-gradient(to right, #f9d771,#f9d771);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Question"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Question"]:after, span.rm-page-ref[data-tag="Question"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Question"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #f9d771;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Question"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #f9d771;
    border-width: 11px;
    margin-top: -11px;
}


```
            - #Help [[Your Name]]
                - ```css
span.rm-page-ref[data-tag="Help"] {
	background-image: linear-gradient(to right, #FF9800,#FF9800);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Help"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Help"]:after, span.rm-page-ref[data-tag="Help"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Help"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #FF9800;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Help"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #FF9800;
    border-width: 11px;
    margin-top: -11px;
}



```
            - #Announcement
                - ```css
span.rm-page-ref[data-tag="Announcement"] {
    color: white !important;
    padding: 3px 5px 3px 5px;
	font-size: 13px;
    line-height: 1em;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FFEFBA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FFFFFF, #FFEFBA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #FC3D39, #FC3D39); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}





```
            - #@ [[Their Name]]
                - ```css
span.rm-page-ref[data-tag="@"] {
	background-image: linear-gradient(to right, #4c8dc9,#4c8dc9);
	background-size: 100%;
    color: #EEF2EE;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="@"] + span[data-link-title] {
     background: #e4ffe3 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="@"]:after, span.rm-page-ref[data-tag="@"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="@"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="@"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}




```
            - #Poll
                - ```css
span.rm-page-ref[data-tag="Poll"] {
    color: white !important;
    padding: 3px 5px 3px 5px;
	font-size: 13px;
    line-height: 1em;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FFEFBA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FFFFFF, #FFEFBA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #5856d6, #5856d6); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}






```
            - #Video
                - ```css
span.rm-page-ref[data-tag="Video"] {
	background-image: linear-gradient(to right, #0D71EB,#0D71EB);
	background-size: 100%;
    color: white;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Video"] + span[data-link-title] {
     background: white !important;
     padding: 2px 5px 2px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border: 1px solid #0D71EB;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Video"]:after, span.rm-page-ref[data-tag="Video"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Video"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #0D71EB;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Video"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #0D71EB;
    border-width: 11px;
    margin-top: -11px;
}




```
            - #[[Daily Writing Prompt]]
                - ```css
span.rm-page-ref[data-tag="Daily Writing Prompt"] {
    color: black !important;
    padding: 3px 5px 3px 5px;
	font-size: 13px;
    line-height: 1em;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #76f264;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #76f264, #76f264);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #76f264, #76f264); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}







```
    5. Tinkering with the above to add preposition forms: (do we want this? maybe let the user base "decide" by their use pattern rather than pick a convention)
        - #Reply-from
            - ```css
span.rm-page-ref[data-tag="Reply-from"] {
	background-image: linear-gradient(to right, #E5E5EA,#E5E511);
	background-size: 100%;
    color: black;
    padding: 5px 3px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Reply-from"] + span[data-link-title] {
     background: #D6B0DD !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Reply-from"]:after, span.rm-page-ref[data-tag="Reply"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Reply-from"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #E5E5EA;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Reply-from"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #E5E5EA;
    border-width: 11px;
    margin-top: -11px;
}
```
        - #Question-for
            - ```css
span.rm-page-ref[data-tag="Question-for"] {
	background-image: linear-gradient(to right, #f9d771,#f9d771);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Question-for"] + span[data-link-title] {
     background: #89F287 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Question-for"]:after, span.rm-page-ref[data-tag="Question"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Question-for"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #FECB2E;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Question-for"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #FECB2E;
    border-width: 11px;
    margin-top: -11px;
}```
        - #Question-from
            - ```css
span.rm-page-ref[data-tag="Question-from"] {
	background-image: linear-gradient(to right, #FECB2E,#f9d771);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Question-from"] + span[data-link-title] {
     background: #89F287 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Question-from"]:after, span.rm-page-ref[data-tag="Question"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Question-from"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #FECB2E;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Question-from"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #FECB2E;
    border-width: 11px;
    margin-top: -11px;
}```
    6. Alerts, and "Seen"
        - ```css
span[data-link-title^="@"] {
        border: 2px solid #a76800 !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="@"]:before {
    color: #000746 !important;
    content: "🚨 "
}

span[data-link-title^="~"] {
        border: 2px solid #02B920 !important;
        padding: 3px 6px 3px 7px;
        margin-right: 1px;
    line-height: 2em;
} 

span[data-link-title^="~"]:before {
    color: #000746 !important;
    content: "✅ (seen) "
}```
    7. Keywords (experimental) - for use in visually demarcating a list of topic hashtags in a header line
        - ```css
[data-tag="kw"] {
  visibility: hidden; 
}

[data-tag="kw"]::after {
  content:"\A";
  white-space: "pre"; 
}

[data-tag="kw"] + [data-tag]::before {
  content: "Keywords: ";
    color: white;
  background-color: #00BCD4;
  font-weight: bold;
  padding-left: 5px;
  padding-right: 3px;
  border-radius: 3px;
  
}
```
    8. (Retired - replaced )Here's a special CSS for custom appearance of the hashtag # `chat` :
NOTE we might change this convention.
        - ```css
span.rm-page-ref[data-tag="chat"]:before {
    content: "👋 "
}

span.rm-page-ref[data-tag="chat"] {
    background: #D7A45463;
    color:  #520365 !important;
    padding: 2px 5px;
    line-height: 2em;
    font-weight: 500;
}```
    9. (Retired) The CSS below will take any link with "@" in front of it and turn it into a bright color. 

Note that CSSes only function if they are the active "version" - these have been turned off by being hidden into inactive "version".

Then, when you've read it, change it to "~" and it will turn green. 
        - (Now if we want to grab somebody's attention make a link with "@" in front of their name.)
            - ```css
span[data-link-title^="@"] {			
   background: #EDA0B5;
}

span[data-link-title^="@"] > span {
   color: #fff !important;
}```
            - ```css
span[data-link-title^="~"] {
   background: #A9EDA0;
}

span[data-link-title^="~"] > span {
   color: #040A55 !important;
}```
    10. CSS code for helping make the [[Daily Notes]] page a little more aesthetically pleasing! (from [[Beau Haan 📌]])
        - #Post [[Your Name]]
            - ```css
span.rm-page-ref[data-tag="Post"] {
	background-image: linear-gradient(to right, #607D8B,#607D8B);
	background-size: 100%;
    color: rgb(255,255,255);
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Post"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Post"]:after, span.rm-page-ref[data-tag="Post"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Post"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #607D8B;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Post"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #607D8B;
    border-width: 11px;
    margin-top: -11px;
}

```
        - #Chat [[Your Name]] #@ [[Beau Haan 📌]]
            - ```css
span.rm-page-ref[data-tag="Chat"] {
	background-image: linear-gradient(to right, #4c8dc9,#4c8dc9);
	background-size: 100%;
    color: #EEF2EE;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Chat"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Chat"]:after, 
span.rm-page-ref[data-tag="Chat"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Chat"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Chat"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}
```
        - #Reply [[Your Name]]
            - ```css
span.rm-page-ref[data-tag="Reply"] {
	background-image: linear-gradient(to right, #E5E5EA,#E5E5EA);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Reply"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Reply"]:after, span.rm-page-ref[data-tag="Reply"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Reply"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #E5E5EA;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Reply"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #E5E5EA;
    border-width: 11px;
    margin-top: -11px;
}

```
        - #Question [[Their Name]]
            - ```css
span.rm-page-ref[data-tag="Question"] {
	background-image: linear-gradient(to right, #f9d771,#f9d771);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Question"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Question"]:after, span.rm-page-ref[data-tag="Question"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Question"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #f9d771;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Question"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #f9d771;
    border-width: 11px;
    margin-top: -11px;
}


```
        - #Help [[Your Name]]
            - ```css
span.rm-page-ref[data-tag="Help"] {
	background-image: linear-gradient(to right, #FF9800,#FF9800);
	background-size: 100%;
    color: black;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Help"] + span[data-link-title] {
     background: #e4ffe3 !important;
     color: #F3F7F2 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Help"]:after, span.rm-page-ref[data-tag="Help"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Help"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #FF9800;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Help"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #FF9800;
    border-width: 11px;
    margin-top: -11px;
}



```
        - #Announcement
            - ```css
span.rm-page-ref[data-tag="Announcement"] {
    color: white !important;
    padding: 3px 5px 3px 5px;
	font-size: 13px;
    line-height: 1em;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FFEFBA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FFFFFF, #FFEFBA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #FC3D39, #FC3D39); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
}





```
        - #@ [[Their Name]]
            - ```css
span.rm-page-ref[data-tag="@"] {
	background-image: linear-gradient(to right, #4c8dc9,#4c8dc9);
	background-size: 100%;
    color: #EEF2EE;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="@"] + span[data-link-title] {
     background: #e4ffe3 !important;
     padding: 3px 5px 3px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="@"]:after, span.rm-page-ref[data-tag="@"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="@"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="@"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #4c8dc9;
    border-width: 11px;
    margin-top: -11px;
}




```
        - #Poll
            - ```css
span.rm-page-ref[data-tag="Poll"] {
    color: white !important;
    padding: 3px 5px 3px 5px;
	font-size: 13px;
    line-height: 1em;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #FFEFBA;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #FFFFFF, #FFEFBA);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #5856d6, #5856d6); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}






```
        - #Video
            - ```css
span.rm-page-ref[data-tag="Video"] {
	background-image: linear-gradient(to right, #0D71EB,#0D71EB);
	background-size: 100%;
    color: white;
    padding: 3px 2px 3px 5px;
    font-size: 13px;
    line-height: 1em;
    border-radius: 3px 0 0 3px;
    position:relative;
}

 span.rm-page-ref[data-tag="Video"] + span[data-link-title] {
     background: white !important;
     padding: 2px 5px 2px 15px;
     font-size: 13px;
     line-height: 1em;
     font-weight: 400;
     border: 1px solid #0D71EB;
     border-radius: 0 3px 3px 0;
     margin-left: -5px;
}


span.rm-page-ref[data-tag="Video"]:after, span.rm-page-ref[data-tag="Video"]:before {
    left: 100%;
    top: 50%;
    border: solid transparent;
    content: " ";
    height: 0;
    width: 0;
    position: absolute;
    pointer-events: none;
}

span.rm-page-ref[data-tag="Video"]:after {
    border-color: rgba(255,255,255,0);
    border-left-color: #0D71EB;
    border-width: 11px;
    margin-top: -11px;
}

span.rm-page-ref[data-tag="Video"]:before {
    border-color: rgba(255,255,255,0);
    border-left-color: #0D71EB;
    border-width: 11px;
    margin-top: -11px;
}




```
        - #[[Daily Writing Prompt]]
            - ```css
span.rm-page-ref[data-tag="Daily Writing Prompt"] {
    color: black !important;
    padding: 3px 5px 3px 5px;
	font-size: 13px;
    line-height: 1em;
    border-radius: 5px 5px 5px 5px;
    position:relative;
background: #76f264;  /* fallback for old browsers */
background: -webkit-linear-gradient(to right, #76f264, #76f264);  /* Chrome 10-25, Safari 5.1-6 */
background: linear-gradient(to right, #76f264, #76f264); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */


}







```
    11. (Experimental) always show the comment icon if using the hidden `{{comment-button}}`. See discussion [here]({{comments: "[[Slipbox]]")
        - ```javascript
/*
Always show the comment button if there are comments
*/
.bp3-icon-comment {
  color: transparent !important;
}
.bp3-icon-comment, .hoveronly{
  opacity:1 !important;
}```
    12. #HIGH-FIVE
        - ```css
span.rm-page-ref[data-tag="HIGH-FIVE"] {
    background: #FFEFBA;
    color: #C95DD9;
    padding: 3px 8px;
    line-height: 2em;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="HIGH-FIVE"]:before {
    content: '🙏 '
}```
    13. #feedback
        - ```css
span.rm-page-ref[data-tag="feedback"] {
    background: #607D8B;
    color: #FFFFFF;
    padding: 3px 8px;
    line-height: 2em;
  	border-radius: 5px 5px 5px 5px;
}

/*
 span.rm-page-ref[data-tag="[[feedback]]: What's working"] {
    background: #609a62;
    color: #FFFFFF;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="[[feedback]]: What could be better"] {
    background: #6775c3;
    color: #FFFFFF;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="[[feedback]]: [[Suggestions]]"] {
    background: #0b8bc5;
    color: #FFFFFF;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}```
    14. #bug-reports
        - ```css
span.rm-page-ref[data-tag="bug-reports"] {
    background: #009688 !important;
    color: #fff !important;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}

span.rm-page-ref[data-tag="bug-reports"]:before {
    content: '🐛 '
}```
    15. #Highlight
        - ```css
span.rm-page-ref[data-tag="Highlight"] {
    background: #FFC107;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}```
    16. #Flag
        - ```css
span.rm-page-ref[data-tag="Flag"] {
    background: #FF9800;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}```
    17. #not-populated
        - ```css
span.rm-page-ref[data-tag="not-populated"] {
    background: #DFDFDF;
    color: #fff;
    padding: 3px 8px;
    line-height: 2em;
    font-weight: 500;
  	border-radius: 5px 5px 5px 5px;
}```
    18.  This CSS makes spaced interval metadata look more beautiful (see: [[spaced repetition]])
        - author: Dave Lu
            - ```css
[data-link-title^="[[interval]]:"], [data-link-title^="[[factor]]:"] {
    display: none;
}
[data-link-title^="[[factor]]:"] ~ [data-link-title]:last-child::before {
    font-style: italic;
    margin-right: 6px;
    padding: 3px 6px;
    border-radius: 12px;
    font-size: smaller;
    white-space: nowrap;
}

[data-link-title^="[[interval]]:"] ~ [data-link-title]:last-child::before {
    content: "review interval: 1+ month";
}


[data-link-title^="[[interval]]:1."] ~ [data-link-title]:last-child::before {
    content: "review interval: 1 day";
}


[data-link-title^="[[interval]]:2."] ~ [data-link-title]:last-child::before {
    content: "review interval: 2 days";
}


[data-link-title^="[[interval]]:3."] ~ [data-link-title]:last-child::before {
    content: "review interval: 3 days";
}


[data-link-title^="[[interval]]:4."] ~ [data-link-title]:last-child::before {
    content: "review interval: 4 days";
}


[data-link-title^="[[interval]]:5."] ~ [data-link-title]:last-child::before {
    content: "review interval: 5 days";
}


[data-link-title^="[[interval]]:7."] ~ [data-link-title]:last-child::before {
    content: "review interval: 1 weeks";
}


[data-link-title^="[[interval]]:8."] ~ [data-link-title]:last-child::before {
    content: "review interval: 1 weeks";
}


[data-link-title^="[[interval]]:9."] ~ [data-link-title]:last-child::before {
    content: "review interval: 1 weeks";
}


[data-link-title^="[[interval]]:10."] ~ [data-link-title]:last-child::before {
    content: "review interval: 1 weeks";
}


[data-link-title^="[[interval]]:11."] ~ [data-link-title]:last-child::before {
    content: "review interval: 1 weeks";
}


[data-link-title^="[[interval]]:12."] ~ [data-link-title]:last-child::before {
    content: "review interval: 1 weeks";
}


[data-link-title^="[[interval]]:13."] ~ [data-link-title]:last-child::before {
    content: "review interval: 1 weeks";
}


[data-link-title^="[[interval]]:14."] ~ [data-link-title]:last-child::before {
    content: "review interval: 2 weeks";
}


[data-link-title^="[[interval]]:15."] ~ [data-link-title]:last-child::before {
    content: "review interval: 2 weeks";
}


[data-link-title^="[[interval]]:16."] ~ [data-link-title]:last-child::before {
    content: "review interval: 2 weeks";
}


[data-link-title^="[[interval]]:17."] ~ [data-link-title]:last-child::before {
    content: "review interval: 2 weeks";
}


[data-link-title^="[[interval]]:18."] ~ [data-link-title]:last-child::before {
    content: "review interval: 2 weeks";
}


[data-link-title^="[[interval]]:19."] ~ [data-link-title]:last-child::before {
    content: "review interval: 2 weeks";
}


[data-link-title^="[[interval]]:20."] ~ [data-link-title]:last-child::before {
    content: "review interval: 2 weeks";
}


[data-link-title^="[[interval]]:21."] ~ [data-link-title]:last-child::before {
    content: "review interval: 3 weeks";
}


[data-link-title^="[[interval]]:22."] ~ [data-link-title]:last-child::before {
    content: "review interval: 3 weeks";
}


[data-link-title^="[[interval]]:23."] ~ [data-link-title]:last-child::before {
    content: "review interval: 3 weeks";
}


[data-link-title^="[[interval]]:24."] ~ [data-link-title]:last-child::before {
    content: "review interval: 3 weeks";
}


[data-link-title^="[[interval]]:25."] ~ [data-link-title]:last-child::before {
    content: "review interval: 3 weeks";
}


[data-link-title^="[[interval]]:26."] ~ [data-link-title]:last-child::before {
    content: "review interval: 3 weeks";
}


[data-link-title^="[[interval]]:27."] ~ [data-link-title]:last-child::before {
    content: "review interval: 3 weeks";
}


[data-link-title^="[[interval]]:28."] ~ [data-link-title]:last-child::before {
    content: "review interval: 4 weeks";
}


[data-link-title^="[[interval]]:29."] ~ [data-link-title]:last-child::before {
    content: "review interval: 4 weeks";
}


[data-link-title^="[[factor]]:"] ~ [data-link-title]:last-child::before {
    border: 1px solid darkgreen;
    color: darkgreen;
    background: honeydew;
}


[data-link-title^="[[factor]]:1."] ~ [data-link-title]:last-child::before {
    border: 1px solid darkred;
    color: darkred;
    background: mistyrose;
}


[data-link-title^="[[factor]]:2."] ~ [data-link-title]:last-child::before {
    border: 1px solid mediumblue;
    color: mediumblue;
    background: lightcyan;
}```
    19. This CSS minimizes the envelope around query results in order to present a cleaner view if you don't want all the context for each result.
        - Note, to "trigger" it, you use the hashtag `#minimal` anywhere in a block, but BEFORE (in front of) the actual `{{query:}}`
        - author: Matt Goldenberg
            - ```css

[data-tag="minimal"] + .rm-query .rm-title-arrow-wrapper, 
[data-tag="minimal"] + .rm-query .zoom-mentions-view {
display:none!important;}
[data-tag="minimal"] + .rm-query .rm-query-title::after {
content: " #minimal"}```
    20. EXPERIMENTAL - This CSS will change the display of blocks that contain `#Zettels`, but ONLY IF you turned on Cato's Roamext javascript
        - author: [[Matt Brockwell/MJB]]
            - ```javascript
[data-tags-up~="Zettels"] > div:nth-child(2) {
border: 1px solid blue;
}```
        - #Zettels
            - yo
            - fro
            - 
