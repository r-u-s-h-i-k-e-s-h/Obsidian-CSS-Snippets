---
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1088453662352887828
cover: "[[img-titlebar - breadcrumb separator.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Titlebar - breadcrumb separator

![](../attachments/img-titlebar%20-%20breadcrumb%20separator.webp)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1088453662352887828
*/

body {
  --file-header-justify: left:
}

.view-header-breadcrumb-separator {
  font-size: 0px;
}

.view-header-breadcrumb-separator::after {
  content: "»";
  font-size: var(--file-header-font-size);
}
```
