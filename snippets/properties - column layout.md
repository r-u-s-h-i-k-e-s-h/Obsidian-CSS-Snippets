---
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1155496243691266158
cover: "[[img-properties - column layout.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Properties - column layout

![](../attachments/img-properties%20-%20column%20layout.webp)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1155496243691266158
*/

[data-type="markdown"] .metadata-properties {
  display: grid;
  grid: auto-flow / 50% 50%;
  gap: 3px 0px;
}

[data-type="markdown"] .metadata-properties .metadata-property-value {
  align-items: start;
}

body {
  --metadata-label-width: 5em;
}
```
