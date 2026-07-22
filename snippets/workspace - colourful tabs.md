---
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1113350168260124743
cover: "[[img-workspace - colourful tabs.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Workspace - colourful tabs

![](../attachments/img-workspace%20-%20colourful%20tabs.webp)

## Snippet

```css
/*
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1113350168260124743

modified the original code in order to make it work for both light and dark mode
*/


.workspace-tab-header-container-inner>.workspace-tab-header {
  background-color: var(--tab-bg) !important;
}

.workspace-tab-header-container-inner>.workspace-tab-header.is-active {
  background-color: var(--tab-active-bg) !important;
  --tab-background-active: var(--tab-active-bg);
}

.workspace-tab-header-container-inner>.workspace-tab-header::after {
  z-index: 1;
}


.theme-dark .workspace-tab-header:nth-child(1) {
  --tab-active-bg: #8e5231;
  --tab-bg: #5b331e;
}

.theme-dark .workspace-tab-header:nth-child(2) {
  --tab-active-bg: #8e313f;
  --tab-bg: #67232d;
}

.theme-dark .workspace-tab-header:nth-child(3) {
  --tab-active-bg: #8e8131;
  --tab-bg: #675e22;
}

.theme-dark .workspace-tab-header:nth-child(4) {
  --tab-active-bg: #313f8e;
  --tab-bg: #212c6a;
}

.theme-dark .workspace-tab-header:nth-child(5) {
  --tab-active-bg: #52318e;
  --tab-bg: #341e5d;
}

.theme-dark .workspace-tab-header:nth-child(6) {
  --tab-active-bg: #318e52;
  --tab-bg: #2f523b;
}


.theme-light .workspace-tab-header:nth-child(1) {
  --tab-active-bg: #ffcca3;
  --tab-bg: #ffe6d1;
}

.theme-light .workspace-tab-header:nth-child(2) {
  --tab-active-bg: #ffb3be;
  --tab-bg: #ffd1d7;
}

.theme-light .workspace-tab-header:nth-child(3) {
  --tab-active-bg: #fff1a3;
  --tab-bg: #fff8d1;
}

.theme-light .workspace-tab-header:nth-child(4) {
  --tab-active-bg: #b3c2ff;
  --tab-bg: #d1daff;
}

.theme-light .workspace-tab-header:nth-child(5) {
  --tab-active-bg: #d5b3ff;
  --tab-bg: #e8d1ff;
}

.theme-light .workspace-tab-header:nth-child(6) {
  --tab-active-bg: #b3ffa2;
  --tab-bg: #d4ffd1;
}
```
