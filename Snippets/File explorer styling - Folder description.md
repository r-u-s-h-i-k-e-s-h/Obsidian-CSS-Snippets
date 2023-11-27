↪[Collection](Collection.md)

# File explorer styling - Folder description

---

- author:: Corellan
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1120300422565994516

---

> _You can change the folder name, and add your own description_

cover:: ![](https://i.imgur.com/UsB7YMQ.png)

```css
/*
author: Corellan
source: https://discord.com/channels/686053708261228577/702656734631821413/1120300422565994516
*/

/* ╔════════════════════════════════════════════════════════════════════════════════════════════════════════[─]═[□]═[×]═╗ */
/* ║ Obsidian Add-On                                                                                                    ║ */
/* ╠══════════════════════════╦═════════════════════════════════════════════════════════════════════════════════════════╣ */
/* ║ Name:                    ║ CreArts Folder-Description                                                              ║ */
/* ║ Version:                 ║ 1.0.0                                                                                   ║ */
/* ║ Author:                  ║ Corellan                                                                                ║ */
/* ║ License:                 ║ MIT                                                                                     ║ */
/* ╚══════════════════════════╩═════════════════════════════════════════════════════════════════════════════════════════╝ */

/* ╔══════════════════════════╦═════════════════════════════════════════════════════════════════════════════[─]═[□]═[×]═╗ */
/* ║ Custom CSS               ║ Vars                                                                                    ║ */
/* ╚══════════════════════════╩═════════════════════════════════════════════════════════════════════════════════════════╝ */

:root {
  --folder-comments-height: 30px;
}

/* ╔══════════════════════════╦═════════════════════════════════════════════════════════════════════════════[─]═[□]═[×]═╗ */
/* ║ Custom CSS               ║ General                                                                                 ║ */
/* ╚══════════════════════════╩═════════════════════════════════════════════════════════════════════════════════════════╝ */

.tree-item-inner::after {
  position: absolute;
  font-size: 10px;
  bottom: 4px;
  left: 25px;
  opacity: 40%;
}

.tree-item .nav-folder:not(.is-collapsed) .tree-item-inner::after {
  color: var(--custom-color-primary);
  opacity: 100;
}

/* ╔══════════════════════════╦═════════════════════════════════════════════════════════════════════════════[─]═[□]═[×]═╗ */
/* ║ Custom CSS               ║ Plugins                                                                                    ║ */
/* ╚══════════════════════════╩═════════════════════════════════════════════════════════════════════════════════════════╝ */

.nav-folder-title[data-count]::after {
  align-self: start;
}

/* ╔══════════════════════════╦═════════════════════════════════════════════════════════════════════════════[─]═[□]═[×]═╗ */
/* ║ Custom CSS               ║ Pseudo                                                                                  ║ */
/* ╚══════════════════════════╩═════════════════════════════════════════════════════════════════════════════════════════╝ */

/* Notes */
[data-path="1 Notes"] .tree-item-inner {
  height: var(--folder-comments-height);
}

[data-path="1 Notes"] .tree-item-inner::after {
  content: "My Personal notes";
}

/* Tasks */
[data-path="2 Tasks"] .tree-item-inner {
  height: var(--folder-comments-height);
}

[data-path="2 Tasks"] .tree-item-inner::after {
  content: "My To-Do's";
}

/* Projects */
[data-path="3 Projects"] .tree-item-inner {
  height: var(--folder-comments-height);
}

[data-path="3 Projects"] .tree-item-inner::after {
  content: "Work in Progress";
}

/* Bookmarks */
[data-path="4 Bookmarks"] .tree-item-inner {
  height: var(--folder-comments-height);
}

[data-path="4 Bookmarks"] .tree-item-inner::after {
  content: "Saved web links";
}

/* Documents */
[data-path="5 Documents"] .tree-item-inner {
  height: var(--folder-comments-height);
}

[data-path="5 Documents"] .tree-item-inner::after {
  content: "Important files";
}

/* Research */
[data-path="6 Research"] .tree-item-inner {
  height: var(--folder-comments-height);
}

[data-path="6 Research"] .tree-item-inner::after {
  content: "Knowledge Hub";
}

/* Resources */
[data-path="8 Resources"] .tree-item-inner {
  height: var(--folder-comments-height);
}

[data-path="8 Resources"] .tree-item-inner::after {
  content: "Files & Resources";
}

/* Templates */
[data-path="9 Templates"] .tree-item-inner {
  height: var(--folder-comments-height);
}

[data-path="9 Templates"] .tree-item-inner::after {
  content: "My Custom Tempaltes";
}
```
