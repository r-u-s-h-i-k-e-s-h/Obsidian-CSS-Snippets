---
author:
  - Bluemoondragon07
source: https://forum.obsidian.md/t/how-to-add-a-custom-image-as-a-background/53416/2?u
cover: "[[img-workspace - custom background image.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Workspace - custom background image

![](../attachments/img-workspace%20-%20custom%20background%20image.webp)

## Snippet

```css
/*
author: Bluemoondragon07
source: https://forum.obsidian.md/t/how-to-add-a-custom-image-as-a-background/53416/2?u
*/

.theme-light .workspace {
  backdrop-filter: brightness(1) blur(5px); /* filter for light mode */
  background-color: transparent;
}
.theme-dark .workspace {
  backdrop-filter: brightness(0.35) blur(5px); /* filter for dark mode */
  background-color: transparent;
}
.horizontal-main-container {
  /* below is the background image. Change it to whatever you want */
  background: url(https://images.unsplash.com/photo-1454496522488-7a8e488e8606?ixlib=rb-4.0.3&ixid=MnwxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8&auto=format&fit=crop&w=2076&q=80);
  background-size: cover;
}
.workspace-split.mod-root {
  background-color: var(--background-primary);
}

body {
  /* the background-primary makes the main note pane completely transparent.
You can change it to be semi-transparent if you want.
I changed background-secondary and divider-width because it
looks a bit cleaner in my opinion. You can delete those modifications if you want.*/
  --background-primary: transparent;
  --background-secondary: transparent;
  --divider-width: 0px;
}
```

## Transparent tab container

```css
.workspace-tab-header-container, .workspace-ribbon.mod-left:before {
  background: transparent;
}
```