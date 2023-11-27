↪[Collection](Collection.md)

# Coloured ribbon

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1147201536171196416

---

cover:: ![](https://i.imgur.com/fTqcg5Y.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1147201536171196416
*/

.workspace-ribbon.side-dock-ribbon.mod-left {
  --titlebar-background-focused: red;
  background-color: var(--titlebar-background-focused);
}
.workspace-ribbon.side-dock-ribbon.mod-left::before,
.workspace-ribbon.side-dock-ribbon.mod-left > .sidebar-toggle-button {
  --titlebar-background: var(--titlebar-background-focused);
}
```

---

> ## _To change colour of icons on the ribbon :)_

```css
.workspace-ribbon.side-dock-ribbon.mod-left .clickable-icon {
  color: white;
}
```
