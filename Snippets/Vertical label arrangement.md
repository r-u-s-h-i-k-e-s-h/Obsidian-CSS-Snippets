↪[Collection](Collection.md)

# Vertical label arrangement

---

- author:: kepano
- source::

---

> \*Extracted from [Minimal Theme](https://github.com/kepano/obsidian-minimal) of **kepano\***

cover:: ![](https://i.imgur.com/EcIdMeF.png)

```css
/* ---------------------------------------------------------------------------

Minimal Theme by @kepano

User interface replacement for Obsidian.

Sponsor my work:
https://www.buymeacoffee.com/kepano

Readme:
https://github.com/kepano/obsidian-minimal

-----------------------------------------------------------------------------

MIT License

Copyright (c) 2020-2023 Stephan Ango (@kepano)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in 
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

*/

.is-fullscreen:not(.colorful-frame) {
  --labeled-nav-top-margin: 0;
}
 {
  --labeled-nav-top-margin: var(--header-height);
}
.is-translucent
  .mod-left-split
  .mod-top
  .workspace-tab-header-container
  .workspace-tab-header-container-inner {
  background-color: transparent;
}
.is-hidden-frameless:not(.is-fullscreen)
  .mod-left-split
  .workspace-tabs.mod-top-left-space
  .workspace-tab-header-container {
  padding-left: 0;
}
.mod-macos .mod-left-split .mod-top .workspace-tab-header-container:before,
.mod-macos.is-hidden-frameless:not(.is-fullscreen)
  .mod-left-split
  .mod-top
  .workspace-tab-header-container:before {
  -webkit-app-region: drag;
  position: absolute;
  width: calc(100% - var(--divider-width));
  height: calc(var(--header-height) - var(--tab-outline-width));
  border-bottom: 0 solid var(--tab-outline-color);
}
.mod-macos.is-hidden-frameless:not(.is-fullscreen)
  .workspace-ribbon.mod-left:not(.is-collapsed) {
  border: none;
  --tab-outline-width: 0px;
}
.colorful-frame.is-hidden-frameless:not(.is-fullscreen)
  .mod-left-split
  .mod-top
  .workspace-tab-header-container:before,
.mod-macos:not(.hider-ribbon)
  .mod-left-split
  .mod-top
  .workspace-tab-header-container:before,
:not(.is-hidden-frameless)
  .mod-left-split
  .mod-top
  .workspace-tab-header-container:before {
  border-bottom: var(--tab-outline-width) solid var(--tab-outline-color);
}
.colorful-frame.is-hidden-frameless:not(.is-fullscreen)
  .workspace-ribbon.mod-left:not(.is-collapsed),
.mod-macos:not(.hider-ribbon) .workspace-ribbon.mod-left:not(.is-collapsed),
:not(.is-hidden-frameless) .workspace-ribbon.mod-left:not(.is-collapsed) {
  --tab-outline-width: 1px;
}
:not(.is-hidden-frameless)
  .mod-left-split
  .mod-top
  .workspace-tab-header-container:before {
  position: absolute;
  top: 0;
  content: " ";
}
.hider-ribbon.mod-macos.is-hidden-frameless:not(.is-fullscreen):not(
    .is-popout-window
  )
  .mod-left-split:not(.is-sidedock-collapsed)
  .workspace-tabs.mod-top-left-space
  .workspace-tab-header-container {
  padding-left: 0;
}
:not(.is-grabbing):not(.is-fullscreen).is-hidden-frameless
  .mod-top
  .workspace-tab-header-container {
  -webkit-app-region: no-drag;
}
.mod-left-split .mod-top .workspace-tab-header-spacer {
  display: none;
}
.mod-left-split .mod-top .workspace-tab-header-inner-title {
  display: inline-block;
  font-weight: 500;
  font-size: var(--font-adaptive-smaller);
}
.mod-left-split .mod-top .workspace-tab-header-container {
  position: relative;
  flex-direction: column-reverse !important;
  height: auto;
  width: 100%;
}

.mod-left-split
  .mod-top
  .workspace-tab-header-container
  .sidebar-toggle-button.mod-left {
  position: absolute;
  justify-content: flex-end;
  padding-right: var(--size-4-2);
  top: 0;
  right: 0;
}

.mod-left-split
  .mod-top
  .workspace-tab-header-container
  .workspace-tab-header-container-inner {
  padding-top: var(--size-4-2);
  margin-top: var(--labeled-nav-top-margin);
  flex-direction: column !important;
  background-color: var(--background-secondary);
}

.mod-left-split
  .mod-top
  .workspace-tab-header-container
  .workspace-tab-container-inner {
  flex-grow: 1;
  gap: 0;
  padding: var(--size-4-2) var(--size-4-3);
}
.mod-left-split .mod-top .workspace-tab-header {
  --icon-color: var(--text-muted);
  --tab-text-color: var(--text-muted);
  --tab-text-color-focused: var(--text-muted);
  padding: 0;
  margin-bottom: 2px;
  border: none;
  height: auto;
}

.mod-left-split .mod-top .workspace-tab-header.is-active:not(:hover) {
  background-color: transparent;
}
.mod-left-split .mod-top .workspace-tab-header.is-active,
.mod-left-split .mod-top .workspace-tab-header:hover {
  opacity: 1;
  --tab-text-color-active: var(--text-normal);
  --tab-text-color-focused: var(--text-normal);
  --tab-text-color-focused-active: var(--text-normal);
  --tab-text-color-focused-active-current: var(--text-normal);
  --icon-color: var(--text-normal);
}

.mod-left-split .mod-top .workspace-tab-header .workspace-tab-header-inner {
  gap: var(--size-2-3);
  padding: var(--size-4-1) var(--size-4-2);
  box-shadow: none;
  border: none;
}

.mod-left-split .mod-top .workspace-tab-header.has-active-menu:hover,
.mod-left-split .mod-top .workspace-tab-header.is-active:hover {
  background-color: transparent;
}

.mod-left-split
  .mod-top
  .workspace-tab-header.is-active:hover
  .workspace-tab-header-inner,
.mod-left-split
  .mod-top
  .workspace-tab-header:not(.is-active):hover
  .workspace-tab-header-inner {
  background-color: var(--nav-item-background-hover);
}

.mod-left-split
  .mod-top
  .workspace-tab-header.is-active
  .workspace-tab-header-inner-icon,
.mod-left-split
  .mod-top
  .workspace-tab-header:hover
  .workspace-tab-header-inner-icon {
  color: var(--icon-color-active);
}
.mod-left-split .mod-top .workspace-tab-header-container {
  border: none;
  padding: 0;
}
body:not(.links-int-on) {
  --link-decoration: none;
}
body:not(.links-ext-on) {
  --link-external-decoration: none;
}
body:not(.sidebar-color) .mod-right-split {
  --background-secondary: var(--background-primary);
}
body:not(.sidebar-color)
  .mod-right-split
  :not(.mod-top)
  .workspace-tab-header-container {
  --tab-container-background: var(--background-primary);
}
```
