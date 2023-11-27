↪[Collection](Collection.md)

# Pinned tab styling

---

- author:: damikiller37
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1122956284040327328

---

cover:: ![](https://i.imgur.com/1Shx6tI.png)

```css
/*
author: damikiller37
source: https://discord.com/channels/686053708261228577/702656734631821413/1122956284040327328
*/

/*
    Icon Only Pinned Tabs Snippet
    Requires Installer version 1.1.9+ due to the use of :has.
*/

/* You don't need this if you you want the pin icons removed */
.workspace
  .mod-root
  .workspace-tab-header[data-type="markdown"]:has(.mod-pinned)
  .workspace-tab-header-inner-icon,
.workspace
  .mod-root
  .workspace-tab-header[data-type="empty"]:has(.mod-pinned)
  .workspace-tab-header-inner-icon {
  display: flex;
}

.workspace-tab-header:has(.mod-pinned) .workspace-tab-header-inner-title {
  display: none;
}

.workspace .mod-root .workspace-tab-header:has(.mod-pinned),
.workspace-tab-header:has(.mod-pinned) .workspace-tab-header-inner {
  flex: unset;
  width: fit-content;
  min-width: unset;
}

/* Keep below if you want to remove the pin icon as well (You can unpin using the right click menu) */

.workspace-tab-header:has(.mod-pinned) .workspace-tab-header-status-container {
  display: none;
}

.workspace-tab-header:has(.mod-pinned) .workspace-tab-header-inner-icon {
  padding-right: unset;
}

.workspace-tab-header:has(.mod-pinned) .workspace-tab-header-inner {
  padding: 0 var(--size-4-2);
}
```
