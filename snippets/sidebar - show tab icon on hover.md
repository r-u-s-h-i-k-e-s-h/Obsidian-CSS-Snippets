---
author:
  - sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1170914511788724254
cover: "[[gif-sidebar - show tab icon on hover.gif]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Sidebar - show tab icon on hover

![](../attachments/gif-sidebar%20-%20show%20tab%20icon%20on%20hover.gif)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1170914511788724254
*/

.workspace-tabs:not(.mod-top) .workspace-tab-header-container {
  height: 0px;
  transition: height 200ms ease-in;

  &:hover {
    height: var(--header-height);
  }

  &::after {
    content: "";
    display: block;
    width: 100%;
    height: var(--size-4-4);
    top: 100%;
    position: absolute;
    z-index: 1;
  }
}
```
