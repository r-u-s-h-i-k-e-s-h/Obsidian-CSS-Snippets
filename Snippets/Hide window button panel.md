↪[Collection](Collection.md)

# Hide window button panel

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1138096095851978833

---

cover:: ![](https://i.imgur.com/Adi7Eyi.gif)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1138096095851978833
*/

/* virtually hide the custom window button panel */
body.is-hidden-frameless:not(:has(.is-right-sidedock-open)) {
  --frame-right-space: 0px;
}
body.is-hidden-frameless:not(:has(.is-right-sidedock-open))
  .titlebar-button-container.mod-right {
  width: 0px;
  transition: width 275ms var(--anim-motion-swing);
}
body.is-hidden-frameless:not(:has(.is-right-sidedock-open))
  .sidebar-toggle-button.mod-right {
  width: var(--ribbon-width);
}
```
