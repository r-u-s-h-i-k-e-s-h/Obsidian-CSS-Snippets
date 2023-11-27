↪[Collection](Collection.md)

# Outline numbering

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1172421139931340810

---

cover:: ![](https://i.imgur.com/lbylqzH.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1172421139931340810
*/

/**************************************
 * Header Counters in ToC pane
 **************************************/

[data-type="outline"] {
  counter-reset: rootLayout;
}
[data-type="outline"] .tree-item .tree-item-self .tree-item-inner::before {
  content: counters(rootLayout, ".") ". ";
  counter-increment: rootLayout;
}
[data-type="outline"] .tree-item-children {
  counter-reset: internalLayout;
}
[data-type="outline"]
  .tree-item-children
  .tree-item
  .tree-item-self
  .tree-item-inner::before {
  content: counters(rootLayout, ".") "." counters(internalLayout, ".") ". " !important;
  counter-increment: internalLayout;
}

/* nested list counting (ex: 1.1, 1.2) */
ol {
  counter-reset: item;
}

ol li {
  display: block;
}

ol li:before {
  content: counters(item, ".") ". ";
  counter-increment: item;
  padding-right: 5px;
}
```
