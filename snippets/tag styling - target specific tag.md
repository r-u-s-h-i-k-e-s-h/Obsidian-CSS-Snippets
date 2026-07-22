---
author:
  - rushi
source:
cover: "[[img-tag styling - target specific tag.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Tag styling - target specific tag

![](../attachments/img-tag%20styling%20-%20target%20specific%20tag.webp)

## Snippet

```css
/*
===================================================================
How to use this for other tags:
1. Replace "fugiat" in [href^="#fugiat"] with your tag name.
2. Replace "fugiat" in .cm-tag-fugiat with your tag name.
3. Change the RGB color values below to your preferred color.
===================================================================
*/

body {
  --custom-tag-rgb: 233, 49, 71;
  --custom-tag-color: rgb(var(--custom-tag-rgb));
}

:is(a.tag[href^="#fugiat"],
  .cm-hashtag-begin.cm-tag-fugiat,
  .cm-hashtag-end.cm-tag-fugiat) {
  background-color: rgba(var(--custom-tag-rgb), 0.1) !important;
  color: var(--custom-tag-color) !important;
  font-weight: 700;
}
```
