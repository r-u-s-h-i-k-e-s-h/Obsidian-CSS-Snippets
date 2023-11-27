↪[Collection](Collection.md)

# Callout styling - 3 callouts

---

- author:: Bluemoondragon07
- source::

---

> _Extracted from [Chime Theme](https://github.com/Bluemoondragon07/chime-theme)_ of **Bluemoondragon07**

**Note**: _You will need **Style settings** plugin_.
cover:: ![](https://i.imgur.com/beca3NA.png)

```css
/*
MIT License

Copyright (c) 2023 Ha'ani Whitlock

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

*/

/* @settings

name: Chime Theme
id: chime-theme
settings:
    -
        id: callout-options
        title: Callouts
        type: heading
        level: 2
        collapsed: true
    -
        id: callout-style
        title: Callout Style
        type: class-select
        allowEmpty: false
        default: callout-normal
        options:
            -
                label: Default
                value: callout-normal
            -
                label: Bordered
                value: callout-bordered
            -
                label: Outlined
                value: callout-outlined
            -
                label: Card
                value: callout-floating   

*/

/* ----- callouts ----- */

.callout,
.callout-normal .callout {
  background-color: rgba(var(--callout-color), 0.17);
  border: none;
  position: relative;
  z-index: 2;
}
.callout-bordered .callout {
  border: 1.2px solid rgb(var(--callout-color));
}
.callout-outlined {
  --callout-title-padding: 5px;
}
.callout-outlined .callout,
.callout-outlined .markdown-source-view.mod-cm6 .callout {
  background-color: transparent !important;
  border: 1.5px solid rgb(var(--callout-color));
  overflow: visible;
  margin: 1.5em 0px 1.5em;
}
.callout-outlined .callout-title {
  background-color: var(--background-primary);
  margin-top: -22.5px;
  margin-left: -0.75em;
  padding: 0 0.5em;
  width: fit-content;
}
.callout-floating .callout,
.callout-floating .markdown-source-view.mod-cm6 .callout {
  margin: 13px 0px;
  border-radius: var(--radius-s);
  border: 1.2px solid rgba(var(--callout-color), 0.7);
  box-shadow: var(--shadow-s);
  background-color: transparent;
  padding: 0px;
}

.callout-floating .callout-title,
.callout-floating .markdown-source-view.mod-cm6 .callout-title {
  background-color: rgba(var(--callout-color), 0.2);
  padding: 10px;
  min-width: 100%;
}
.callout-floating .callout-content,
.callout-floating .markdown-source-view.mod-cm6 .callout-content {
  padding: 0px 10px;
}
```
