---
author: ebullient
source: https://discord.com/channels/686053708261228577/702656734631821413/930097778741354517
cover: "[[img-sidebar - rainbow tab icon.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Sidebar - rainbow tab icon

![](../attachments/img-sidebar%20-%20rainbow%20tab%20icon.webp)

## Snippet

```css
/*
author: ebullient
source: https://discord.com/channels/686053708261228577/702656734631821413/930097778741354517

===================================================================
note: To target a different note/tab, change the [aria-label="colors"] value to match the exact title of your note (e.g., [aria-label="Daily Note"])
===================================================================
*/

.workspace-tab-header[aria-label="colors"]
  > .workspace-tab-header-inner
  > .workspace-tab-header-inner-icon {
  width: 17px;
  height: 17px;
  background: linear-gradient(to right, red, orange, yellow, green, cyan, blue, violet);
  border-radius: 4px;
}

/* Hides the default SVG icon so only the color block displays */
.workspace-tab-header[aria-label="colors"]
  > .workspace-tab-header-inner
  > .workspace-tab-header-inner-icon
  > svg {
  display: none;
}
```
