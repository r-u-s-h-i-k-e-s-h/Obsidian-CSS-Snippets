---
author:
  - Corellan
source: https://discord.com/channels/686053708261228577/702656734631821413/1120163092752510976
cover: "[[img-explorer styling - custom folder group header.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Explorer styling - custom folder group header

![](../attachments/img-explorer%20styling%20-%20custom%20folder%20group%20header.webp)

## Snippet

```css
/*
author: Corellan
source: https://discord.com/channels/686053708261228577/702656734631821413/1120163092752510976
modified for obsidian layout compatibility (v1.12.7)

===================================================================
How to customize this for your own folder groups:
1. "nth-child(X)" targets the folder position in your root sidebar.
   For example, :nth-child(3) targets the 3rd root item.
2. Change the text inside content: "YOUR HEADER"; to change the title.
===================================================================
*/

.nav-files-container>div>.nav-folder::after {
  position: relative;
  left: var(--layout-margin);
  font-size: var(--font-adaptive-smallest, 11px);
  font-weight: 500;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  color: var(--text-muted);
}

/* Group Headers */
.nav-files-container>div>.nav-folder:nth-child(3)::after {
  content: "Private";
}

.nav-files-container>div>.nav-folder:nth-child(7)::after {
  content: "Assets";
}

.nav-files-container>div>.nav-folder:nth-child(9)::after {
  content: "Sorting";
}
```
