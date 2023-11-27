↪[Collection](Collection.md)

# Sidenote callout 02

---

- author:: FireIsGood
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1145768722431225926

---

cover:: ![](https://i.imgur.com/EfL7ROv.gif)

```css
/*
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1145768722431225926
*/

:root {
  --tooltip-size: 250px;
}

.markdown-preview-view {
  container-name: page;
  container-type: inline-size;
}

@container page (width > 1200px) {
  .markdown-reading-view .callout[data-callout="epic"] {
    --p-spacing: 0;
    position: absolute;
    width: var(--tooltip-size);
    translate: calc(-1 * (var(--tooltip-size) + 1rem)) 0;
  }
}
```
