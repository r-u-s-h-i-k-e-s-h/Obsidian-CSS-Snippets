---
author:
  - kneecaps
source: https://discord.com/channels/686053708261228577/702656734631821413/1110959351952318474
cover: "[[img-canvas styling - brutalist.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Canvas styling - brutalist

![](../attachments/img-canvas%20styling%20-%20brutalist.webp)

## Snippet

```css
/*
author: kneecaps
source: https://discord.com/channels/686053708261228577/702656734631821413/1110959351952318474
*/

.canvas-node:not(.canvas-node-group) {
  background-color: var(--background-primary);
  border-radius: 0px;
  --shadow-border-themed-inset: inset 0 0 0 1px rgb(var(--canvas-color));
  --shadow-border-themed: 0 0 0 2px rgb(var(--canvas-color));
  position: absolute;
  width: 0;
  height: 0;
  box-shadow: 10px 10px 0 -2.5px #fff, 10px 10px 0 0 var(--text-normal);
  border: 2.5px solid var(--text-normal);
}

.canvas-node:not(.canvas-node-group) .canvas-node-content {
  background: var(--background-primary);
}

.canvas-node:not(.canvas-node-group):before {
  background: rgb(var(--canvas-color));
  content: "";
  position: absolute;
  top: 10px;
  left: 10.1px;
  width: 100%;
  height: 100%;
  border-radius: 0px;
}

.canvas-node-container {
  background: transparent;
  border-radius: 0px;
  border: none;
  contain: strict;
  display: flex;
  height: 100%;
}

.canvas-node-content.markdown-embed>.markdown-embed-content>.markdown-preview-view .markdown-preview-pusher+div>*:first-child {
  color: rgb(var(--canvas-color));
}
```
