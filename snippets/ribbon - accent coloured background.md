---
author:
  - sailKite
  - rushi
source: https://discord.com/channels/686053708261228577/702656734631821413/1147201536171196416
cover: "[[img-ribbon - accent coloured background.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Ribbon - accent coloured background

![](../attachments/img-ribbon%20-%20accent%20coloured%20background.webp)

## Snippet

```css
/*
Original Author: sailKite
Source: https://discord.com/channels/686053708261228577/702656734631821413/1147201536171196416
Modified By: rushi

Note: Tweaked the original code for a cleaner look
*/

.workspace-ribbon.side-dock-ribbon.mod-left {
  --titlebar-background-focused: var(--color-accent);
  background-color: var(--titlebar-background-focused);
}

.workspace-ribbon.side-dock-ribbon.mod-left::before,
.workspace-ribbon.side-dock-ribbon.mod-left>.sidebar-toggle-button {
  --titlebar-background: var(--titlebar-background-focused);
  margin-left: -1px;
  padding-right: 0;
}

.workspace-ribbon.side-dock-ribbon.mod-left .clickable-icon {
  color: white;
}

.workspace-ribbon.mod-left::before {
    border-bottom: var(--tab-outline-width) solid transparent;
}
```
