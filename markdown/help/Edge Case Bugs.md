- when this block is on [[roam/css]] we get a syntax error appearing in the script loader -- probably has to do with how we're parsing for tags...
    - `[[.rm-g]]`
        - #[[.rm-g]] #[[Semantic Classes]]
            - css
                - ```javascript
.rm-g.rm-not-focused {
  position: relative;
}
.rm-g.rm-not-focused .rm-page-ref[data-tag=".rm-g"] {
  display: none;
  color: green;
}
.rm-g.rm-not-focused .rm-block {
  border: none;
  margin: 0px;
  background-color: #F5F8FA;
}
.rm-g.rm-not-focused.rm-block--open {
  display: flex;
  flex-direction: row;
}
.rm-g.rm-not-focused.rm-block--open.rm-not-focused > .rm-block__self {
  position: absolute;
  border-left: 2px solid #BFCCD6;
  border-radius: 20px 0px 0px 20px;
  width: 40px;
  top: 0;
  bottom: 0;
  overflow: hidden;
}
.rm-g.rm-not-focused.rm-block--open.rm-not-focused > .rm-block__self .rm-block__controls {
  display: none;
}
.rm-g.rm-not-focused.rm-block--open.rm-not-focused > .rm-block__self > .rm-block__input--view {
  position: absolute;
  z-index: 9;
  background-color: #394B59;
  right: 0px;
  left: 0;
  top: 0;
  bottom: 0;
  transform: rotate(90deg) translateY(-1em);
  transform-origin: top left;
  font-size: 0.8em;
  max-height: 1em;
  min-width: 100vh;
}
.rm-g.rm-not-focused.rm-block--open > .rm-block__children {
  margin-left: 0px !important;
  min-width: 100%;
}
.rm-g.rm-not-focused.rm-block--open.rm-focused .rm-block__self {
  flex: 1 1 100%;
  width: 100%;
}
.rm-g.rm-not-focused.rm-block--closed > .rm-block__self .rm-block-separator {
  height: 100%;
  border-left: 2px solid #8A9BA8;
  border-radius: 50px;
}```
- 
