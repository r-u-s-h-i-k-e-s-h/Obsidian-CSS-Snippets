---
author: the.tablet
source: https://discord.com/channels/686053708261228577/702656734631821413/1261066509565038622
cover: "[[img-callout styling - bordered hollow.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - bordered hollow

![](../attachments/img-callout%20styling%20-%20bordered%20hollow.webp)

## Snippet

```css
/*
author: the.tablet
source: https://discord.com/channels/686053708261228577/702656734631821413/1261066509565038622
*/

.callout {
  background-color: transparent;
  border: 2px solid rgb(var(--callout-color));
}

.callout:not(.callout.is-collapsed)>.callout-title {
  border-bottom: 2px solid rgb(var(--callout-color)) !important;
  margin-inline-start: -1.5em;
  margin-inline-end: -1em;
  padding: 0 1em;
  padding-bottom: 0.5em;
}
```
