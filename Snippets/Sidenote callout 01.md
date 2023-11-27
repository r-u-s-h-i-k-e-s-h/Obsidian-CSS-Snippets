↪[Collection](Collection.md)

# Sidenote callout 01

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1155147566615367680

---

cover:: ![](https://i.imgur.com/z64RVEY.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1155147566615367680
*/

/* aside functionality as a custom callout */
:is(.markdown-source-view .cm-callout, div:not([class])):has(
    > .callout[data-callout-metadata*="aside"]
  ) {
  position: relative;
  overflow: visible;
  contain: none !important;
}
.callout[data-callout-metadata*="aside"] {
  --aside-width: 200px;
  --aside-offset: var(--size-4-4);
  position: absolute;
}
.callout[data-callout-metadata*="aside-l"] {
  left: calc(-1 * (var(--aside-width) + var(--aside-offset)));
  right: calc(100% + var(--aside-offset));
}
.callout[data-callout-metadata*="aside-r"] {
  left: calc(100% + var(--aside-offset));
  right: calc(-1 * (var(--aside-width) + var(--aside-offset)));
}
@media (hover: hover) {
  .markdown-source-view.mod-cm6
    .cm-embed-block:has(> div > [data-callout-metadata*="aside"]):hover {
    overflow: visible;
  }
}
```

---

## How to use

```md
> [!bug|aside-r]
> your text here
```

```md
> [!bug|aside-l]
> your text here
```
