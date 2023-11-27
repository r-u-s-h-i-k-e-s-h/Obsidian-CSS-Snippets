↪[Collection](Collection.md)

# Ribbon styling - Hide ribbon on collapse

---

- author:: matekusu
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1147232919946022943

---

cover:: ![](https://i.imgur.com/FCwk5lw.gif)

```css
/*
author: matekusu
source: https://discord.com/channels/686053708261228577/702656734631821413/1147232919946022943
*/

/* Immersive Ribbon Menu */
.workspace-ribbon.mod-left {
  background-color: transparent; /*c myn: hides weird flashing in default theme when opening */
  transition: all 0.2s ease-in-out;
  &::before {
    border-bottom-color: transparent;
    transition: all 0.2s ease-in-out;
  }
  &.is-collapsed {
    border-right-color: transparent;
    transition: all 0.2s ease-in-out;
    &::before {
      border-bottom-color: var(--tab-outline-color);
      transition: all 0.2s ease-in-out;
    }
    &:hover > :nth-child(n + 2) {
      opacity: 1;
      transition: all 0.2s ease-in-out;
    }
    &:not(:hover) > :nth-child(n + 2) {
      opacity: 0;
      transition: all 0.2s ease-in-out;
    }
  }
}

/* Immersive Sidebar Collapse */
.workspace-split.mod-horizontal:is(.mod-left-split, .mod-right-split) {
  &.is-sidedock-collapsed {
    .workspace-tabs .workspace-tab-header-container,
    .workspace-tabs .workspace-tab-container,
    .workspace-tabs .workspace-leaf-resize-handle,
    .workspace-tabs.mod-top .workspace-tab-header-inner {
      opacity: 0;
      transition: all 0.2s ease-in-out;
    }
    .workspace-tabs.mod-top .workspace-tab-header-container {
      opacity: 1;
    }
  }
}
```
