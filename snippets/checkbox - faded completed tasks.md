---
author: skantola
source: https://discord.com/channels/686053708261228577/702656734631821413/930104927009779823
cover: "[[img-checkbox - faded completed tasks.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Checkbox - faded completed tasks

![](../attachments/img-checkbox%20-%20faded%20completed%20tasks.webp)

## Snippet

```css
/*
author: skantola
source: https://discord.com/channels/686053708261228577/702656734631821413/930104927009779823
*/

/* ----------------------- */
/* Faded emoji in ✓ tasks */
/* github.com/sampokantola */
/* ----------------------- */
ul>li.task-list-item p {
  text-indent: -1.5em;
}

ul>li.task-list-item.is-checked {
  position: relative;
  filter: url();
}

ul>li.task-list-item.is-checked::after {
  content: "";
  position: absolute;
  display: inline-block;
  backdrop-filter: grayscale();
  width: 100%;
  height: 100%;
  top: 0;
  left: 0;
}

.markdown-source-view.mod-cm6 .HyperMD-task-line[data-task]:not([data-task=" "]) span {
  filter: grayscale();
}
```
