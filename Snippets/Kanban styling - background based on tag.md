↪[Collection](Collection.md)

# Kanban styling - background based on tag

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1173968522372722689

---

cover:: ![](https://i.imgur.com/p9i7Mdb.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1173968522372722689
*/

/* --- Kanban With Background Color Based On Tag --- */
/* use this to style the card background and text */
.kanban-plugin__item.has-tag-someTag,
.has-tag-someTag
  :is(
    .kanban-plugin__item-content-wrapper,
    .kanban-plugin__item-title-wrapper
  ) {
  background-color: red !important;
  color: black;
}

/* use this to style the tag bubble at the bottom of the card */
a[href="#someTag"].kanban-plugin__item-tag {
  background-color: yellow;
  color: green !important;
  font-weight: bold;
}
```
