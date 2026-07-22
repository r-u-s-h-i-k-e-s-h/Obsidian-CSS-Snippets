---
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1172421139931340810
cover: "[[img-sidebar - outline numbering.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Sidebar - outline numbering

![](../attachments/img-sidebar%20-%20outline%20numbering.webp)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1172421139931340810
note: original snippet is modified for obsidian v1.12.7
*/

[data-type="outline"] .workspace-leaf-content-hrx {
  counter-reset: outline-c;
}

[data-type="outline"] .tree-item {
  counter-increment: outline-c;
}

[data-type="outline"] .tree-item-children {
  counter-reset: outline-c;
}

[data-type="outline"] .tree-item-self .tree-item-inner::before {
  content: counters(outline-c, ".") ". ";
  font-variant-numeric: tabular-nums;
}
```
