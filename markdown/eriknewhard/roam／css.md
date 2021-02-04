- Variables
    - No CSS
        ```css
:root {
  --tag-actual-height: 17px;
  --tag-actual-padding-horizontal: 3px;
  --hashtag-width: 9px;
  --tag-icon-padding: 1px;
  
  --reference-bg-color: #F5F8FA;
  --embed-bg-color: #EBF1F5;
}```
    - CALCULATIONS
        ```css
:root {
  --spacing-after-icon: var(--tag-actual-padding-horizontal);
  
  /* icon size */
  --tag-icon-height: calc(var(--tag-actual-height) - (2 * var(--tag-icon-padding)));
  --tag-icon-width: var(--tag-icon-height);
  
  /* hashtag blocking */
  --hash-blocking-bg-width: calc(var(--tag-icon-width) + var(--spacing-after-icon));
  --tag-extra-padding-left: calc(var(--tag-actual-padding-horizontal) + var(--hash-blocking-bg-width) - var(--hashtag-width));
}```
- 
- #[[Tweeted]]
    ```css
span.rm-page-ref[data-tag="Tweeted"],
span.rm-page-ref[data-tag="Retweeted"],
span.rm-page-ref[data-tag="Tweet draft"] {
  color: rgb(29, 161, 242) !important;
  font-weight: 700;
  background-color: white !important;

  position: relative;
  padding-left: var(--tag-extra-padding-left);
  padding-right: var(--tag-actual-padding-horizontal);
}

span.rm-page-ref[data-tag="Tweeted"]:before,
span.rm-page-ref[data-tag="Retweeted"]:before,
span.rm-page-ref[data-tag="Tweet draft"]:before {
  background: white;

  content: '';
  width: var(--hash-blocking-bg-width);
  height: var(--tag-icon-height);
  position: absolute;
  left: var(--tag-actual-padding-horizontal);
  top: var(--tag-icon-padding);
}

span.rm-page-ref[data-tag="Tweeted"]:after,
span.rm-page-ref[data-tag="Retweeted"]:after,
span.rm-page-ref[data-tag="Tweet draft"]:after {
  background: url('https://twitter.com/favicon.ico') no-repeat;
  
  content: '';
  width: var(--tag-icon-width);
  height: var(--tag-icon-height);
  position: absolute;
  left: var(--tag-actual-padding-horizontal);
  top: 0;
  margin-top: var(--tag-icon-padding);
  background-size: var(--tag-icon-width) var(--tag-icon-height);
}

.rm-reference-item span.rm-page-ref[data-tag="Tweeted"],
.rm-reference-item span.rm-page-ref[data-tag="Retweeted"],
.rm-reference-item span.rm-page-ref[data-tag="Tweet draft"] {
  background-color: var(--reference-bg-color) !important;
}

.rm-reference-item span.rm-page-ref[data-tag="Tweeted"]::before,
.rm-reference-item span.rm-page-ref[data-tag="Retweeted"]::before,
.rm-reference-item span.rm-page-ref[data-tag="Tweet draft"]::before {
  background-color: var(--reference-bg-color) !important;
}

.rm-embed-container span.rm-page-ref[data-tag="Tweeted"],
.rm-embed-container span.rm-page-ref[data-tag="Retweeted"],
.rm-embed-container span.rm-page-ref[data-tag="Tweet draft"], {
  background-color: var(--embed-bg-color) !important;
}

.rm-embed-container span.rm-page-ref[data-tag="Tweeted"]::before,
.rm-embed-container span.rm-page-ref[data-tag="Retweeted"]::before,
.rm-embed-container span.rm-page-ref[data-tag="Tweet draft"]::before {
  background-color: var(--embed-bg-color) !important;
}```
- 
