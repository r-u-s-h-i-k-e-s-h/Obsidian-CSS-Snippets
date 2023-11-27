↪[Collection](Collection.md)

# Callout styling - Scroller callout

---

- author:: FireIsGood
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1103116637529456720

---

cover:: ![](https://i.imgur.com/nSnLYXO.gif)

```css
/*
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1103116637529456720
*/

[data-callout="scroller"] {
  --callout-color: 255, 0, 0; /* Replace this with rgb values */
  --shown-line-count: 8; /* Replace this with the number of text lines to show */
}
[data-callout="scroller"] .callout-title {
  display: none;
}
[data-callout="scroller"] .callout-content {
  max-height: calc(var(--line-height-normal) * 1rem * var(--shown-line-count));
}
```

---

## How to use

```md
> [!scroller]
> Generating random paragraphs can be an excellent way for writers to get their creative flow going at the beginning of the day. The writer has no idea what topic the random paragraph will be about when it appears. This forces the writer to use creativity to complete one of three common writing challenges. The writer can use the paragraph as the first one of a short story and build upon it. A second option is to use the random paragraph somewhere in a short story they create. The third option is to have the random paragraph be the ending paragraph in a short story. No matter which of these challenges is undertaken, the writer is forced to use creativity to incorporate the paragraph into their writing.
```
