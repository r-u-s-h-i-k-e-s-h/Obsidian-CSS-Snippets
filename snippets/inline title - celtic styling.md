---
author:
  - sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1163153997465653370
cover: "[[img-inline title - celtic styling.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Inline title - celtic styling

![](../attachments/img-inline%20title%20-%20celtic%20styling.webp)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1163153997465653370
*/

.inline-title {
  display: flex;
  justify-content: center;
  gap: 2.5%;
  align-items: center;

  &::before,
  &::after {
    content: "";
    background-image: url("https://svgsilh.com/png-1024/149731.png");
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
    flex: 0 0 5em;
    aspect-ratio: 1;
  }

  &::after {
    scale: -1 1;
  }
}
```
