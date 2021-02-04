- [[Custom User Styles]]
    - use [[Stylus]] 
        - https://chrome.google.com/webstore/detail/stylus/clngdbkpkpeebahjckkjfobafhncgmne?hl=en
        - ```@-moz-document url("https://roamresearch.com/#/app/malcolm"), url-prefix("https://roamresearch.com/#/app/malcolm/") {
.roam-sidebar-content > .rc-h-box:first-child:after {
    color: white;
    padding-left: 10px;
}
.roam-topbar .rc-h-box > div:nth-child(3) {
    padding-left: 30px;
}
​
.roam-sidebar-content > .rc-h-box:first-child:after,
.roam-topbar .rc-h-box > div:nth-child(3):after {
    content: "malcolm";
}
​
.roam-sidebar-content {background: #321;}
.roam-topbar {background: #b56d0022}
}
​
@-moz-document url-prefix("https://roamresearch.com/#/app/malcolmocean") {
.roam-sidebar-content > .rc-h-box:first-child:after {
    color: white;
    padding-left: 10px;
}
.roam-topbar .rc-h-box > div:nth-child(3) {
    padding-left: 30px;
    color: white
}
​
.roam-sidebar-content > .rc-h-box:first-child:after,
.roam-topbar .rc-h-box > div:nth-child(3):after {
/*    content: "malcolmocean";*/
    content: "";
    display: inline-block;
    position: relative;
    
    width: 100px;
    height: 25px;
    background: url(https://malcolmocean.com/wp-content/themes/minx/img/logo.png) center no-repeat;
    background-size: 100px 25px;
    margin-left: 10px;
}
.roam-topbar .rc-h-box > div:nth-child(3):after {
    top: 2px;
}
​
.roam-sidebar-content {background: #591420;}
.roam-topbar {background: #f2c6ce}
​
.roam-sidebar-content {
    background: url(https://malcolmocean.com/wp-content/themes/minx/img/footer.png);
    background-position: center bottom;
}
.roam-topbar {
    background: url(https://malcolmocean.com/wp-content/themes/minx/img/header.png);
    background-size: 700px;
    box-shadow: 0 1.5px 4px rgba(0,0,0,0.7)
}
​
.roam-topbar .bp3-button:not([class*="bp3-intent-"])::before {
    color: black
}
}```
