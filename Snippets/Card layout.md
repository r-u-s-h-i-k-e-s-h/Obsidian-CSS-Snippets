↪[Collection](Collection.md)

# Card layout

---

- author:: sai1494
- source:: https://discord.com/channels/686053708261228577/744933215063638183/1034885176968347668

---

cover:: ![](https://i.imgur.com/ZRV5Y1v.png)

```css
/*
author: sai1494
source: https://discord.com/channels/686053708261228577/744933215063638183/1034885176968347668
*/

html * {
  --titlebar-background: transparent !important;
  --titlebar-background-focused: transparent !important;
  --ribbon-background: transparent !important;
  --ribbon-background-collapsed: transparent !important;
  --collapsed-right-margin: 24px;
}

.workspace {
  background-color: var(--background-secondary);
}

.workspace-ribbon,
.workspace-leaf-resize-handle {
  border: none !important;
}

.workspace-leaf {
  border-radius: 8px;
  border: 0;
}

/* Adding border to the main workspace leaf */
.mod-root .workspace-leaf {
  border: 1px solid var(--divider-color);

  /* contain is to fix the border-right getting cut off when right collapsed */
  contain: size !important;
}

/* contain is to fix the border-right getting cut off when right collapsed */
.workspace-split.mod-root .view-content {
  background-color: inherit !important;
}

.mod-root .view-content {
  border-top: 1px solid var(--divider-color);
}

/* This is the gap between split workspaces */
.workspace-split {
  background-color: transparent !important;
  gap: 0px 8px;
}

/* .workspace-split.mod-root {
  gap: 8px;
} */

body .mod-right-split {
  --background-secondary: initial !important;
}

.workspace-tab-header-container {
  background-color: var(--background-secondary);
  border-bottom: initial;
}

.workspace-tab-header.is-active {
  box-shadow: initial;
}

.workspace-ribbon.mod-left:before {
  border-bottom: initial;
}

.workspace-ribbon.mod-left.is-collapsed {
  --titlebar-background-focused: transparent !important;
}

.status-bar {
  --status-bar-position: static;
  /* --status-bar-radius: 0; */
  /* --status-bar-border-width: 0 !important; */
  /* --status-bar-background: var(--background-secondary); */
  /* --status-bar-border-color: var(--ui1); */
  border: none;
  border-radius: 0%;
}

/* Fixing indent guides alignment in reader mode */
.markdown-rendered.show-indentation-guide li > ul::before,
.markdown-rendered.show-indentation-guide li > ol::before {
  left: -12px;
}

/* Used to apply a right margin when the right sidebar is collapsed */
.workspace:not(.is-right-sidedock-open) > .mod-root {
  margin-right: var(--collapsed-right-margin) !important;
}

.workspace:not(.is-right-sidedock-open) * .sidebar-toggle-button {
  margin-right: calc(0px - var(--collapsed-right-margin)) !important;
}

.mod-root .workspace-tab-header-container:after {
  margin-right: calc(0px - var(--collapsed-right-margin));
}

/* Used for left aligning the document breadcrumb */
.view-header-title-container {
  justify-content: left;
  opacity: initial;
}

/* Fix tag misalignment */
.cm-hashtag-begin {
  display: inline-block;
  line-height: unset !important;
}

/* Fix tag misalignment */
.cm-hashtag-end {
  display: inline-block;
}

/* Font clarity adjustment */
body {
  word-spacing: -0.04rem;
  letter-spacing: 0.01rem;
  -webkit-font-smoothing: antialiased !important;
}
```
