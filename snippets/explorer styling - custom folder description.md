---
author: Corellan
source: https://discord.com/channels/686053708261228577/702656734631821413/1120300422565994516
cover: "[[img-explorer styling - custom folder description.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Explorer styling - custom folder description

![](../attachments/img-explorer%20styling%20-%20custom%20folder%20description.webp)

## Snippet

```css
/*
author: Corellan
source: https://discord.com/channels/686053708261228577/702656734631821413/1120300422565994516

===================================================================
How to customize this for your own folders:
1. Replace the folder path in [data-path="Your Folder Name"]
   (Note: If it's a subfolder, use the full path like "Parent/Subfolder")
2. Change the text inside content: "Your description here";
===================================================================
*/

:root {
  --folder-comments-height: 30px;
}

/* General Layout Adjustments */
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

.nav-folder-title[data-count]::after {
  align-self: start;
}

/* -----------------------------------------------------------------
   Custom Folder Entries
   ----------------------------------------------------------------- */

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
  content: "My Custom Templates";
}
```
