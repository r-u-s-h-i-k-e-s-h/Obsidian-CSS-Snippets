---
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1096492008526319677
cover: "[[img-image styling - grid layout.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Image styling - grid layout

> Only works in reading mode

![](../attachments/img-image%20styling%20-%20grid%20layout.webp)

## Snippet

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

.cm-line:not(.cm-active):has(.image-embed ~ .image-embed) :is(.cm-widgetBuffer, span) {
  display: none !important;
}

/* Makes a highlighted line shrink the image */
:root:root .cm-line.cm-active>.image-embed {
  width: 100px;
  display: inline-block;
}

/* Centers the image if it is modified */
:root:root .cm-line:not(.cm-active)>.image-embed,
p>.image-embed {
  display: flex;
  place-items: center;
  flex-direction: column;
}
```

## How to use

```md
![[img 01.jpg]]
![[img 02.jpg]]
![[img 03.jpg]]

![[img 03.jpg]]
![[img 01.jpg]]
![[img 02.jpg]]
```