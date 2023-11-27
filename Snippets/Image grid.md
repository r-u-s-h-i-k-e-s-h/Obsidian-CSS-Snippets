↪[Collection](Collection.md)

# Image grid

---

- author:: FireIsGood
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1096492008526319677

---

> _Only works in reading mode_

cover:: ![](https://i.imgur.com/WVW4rKV.png)

```css
/*
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1096492008526319677
*/

/* Makes multiple images on the same line appear in a flex grid */
.cm-line:not(.cm-active):has(.image-embed ~ .image-embed),
p:has(.image-embed ~ .image-embed) {
  display: flex;
  gap: 0.5rem;
}
.cm-line:not(.cm-active):has(.image-embed ~ .image-embed)
  :is(.cm-widgetBuffer, span) {
  display: none !important;
}
/* Makes a highlighted line shrink the image */
:root:root .cm-line.cm-active > .image-embed {
  width: 100px;
  display: inline-block;
}
/* Centers the image if it is modified */
:root:root .cm-line:not(.cm-active) > .image-embed,
p > .image-embed {
  display: flex;
  place-items: center;
  flex-direction: column;
}
```

---

## Usage

```md
![[image 01.jpg]]
![[image 01.jpg]]
![[image 01.jpg]]
![[image 01.jpg]]
```
