---
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1134127383872536576
cover: "[[gif-callout styling - collapsible image caption.gif]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - collapsible image caption

![](../attachments/gif-callout%20styling%20-%20collapsible%20image%20caption.gif)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1134127383872536576
*/

/* image caption collapsible callout */
.callout[data-callout="img-caption"] {
  --callout-color: none;
  --callout-icon: none;
  padding: 12px 0px;
}

.callout[data-callout="img-caption"]>.callout-title {
  font-size: 0px;
  justify-content: center;
}

.callout[data-callout="img-caption"]>.callout-title> :is(.callout-icon, .callout-fold) {
  display: none;
}

.callout[data-callout*="img-caption"]>.callout-content {
  text-align: center;
}
```

## How to use

```md
> [!img-caption]+ ![[img]]
> caption...
```
