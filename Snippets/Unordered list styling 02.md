↪[Collection](Collection.md)

# Unordered list styling 02

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1140761432082886707

---

cover:: ![](https://i.imgur.com/ZicMDLz.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1140761432082886707
*/

:is(.cm-formatting-list-ul, .markdown-rendered ul > li) > .list-bullet::after {
  border: 1px solid var(--list-marker-color);
}
:is(
    ul:not(li > ul) > li > ul > li,
    ul:not(li > ul) > li > ul > li > ul > li > ul > li,
    ul:not(li > ul) > li > ul > li > ul > li > ul > li > ul > li > ul > li,
    ul:not(li > ul)
      > li
      > ul
      > li
      > ul
      > li
      > ul
      > li
      > ul
      > li
      > ul
      > li
      ul
      > li
      > ul
      > li
  )
  > .list-bullet::after,
:is(
    .HyperMD-list-line-2,
    .HyperMD-list-line-4,
    .HyperMD-list-line-6,
    .HyperMD-list-line-8
  )
  .cm-formatting-list-ul
  > .list-bullet::after {
  background-color: transparent;
}
```
