- Custom CSS for tags was previously pretty difficult
- # ~~The Old Version~~
    - You had to remember to use `data-page-links` or `data-page-path-links` as a css selector -- which even our team often could not remember without inspecting the html.
        - {{embed: ((wh4I_Y64t))}}
            - #rm-blue-border--children
                - a
                - b
                - c
- # The New Version
    - Now if you want to create a tag that will apply custom styling to just the block you're on - it is much easier -- just put `.` in the name of the link or tag
        - from [[roam/css]] page
            - {{embed: ((AgZ2IQzp4))}}
        - Hover on me to see the custom block tag#.bblue 
        - 
- "```css
.green  {
  margin: 2px;
  background-color: green;
  color: white;
}```"
-  and more. #.bblue #.green 
    - A
    - B
