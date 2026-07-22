---
author: zakum
source: https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets/pull/15
cover: "[[img-workspace - macos like titlebar buttons.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Workspace - MacOS like titlebar buttons

![](../attachments/img-workspace%20-%20macos%20like%20titlebar%20buttons.webp)

## Snippet

```css
/*
author: zakum
source: https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets/pull/15

*/

/* MacOS Minimize/Maximize/Close buttons by @.zakum */
/* I don't know how MacOS buttons function on hover and whatnot so I just kept the default Obsidian behavior. */

/* Known issue: In graph view, the filters pane is shifted 1px vertically when toggling this snippet. Maybe some other things as well because the code plays with borders and heights a bit. */

:root {
  --macOS-nav-dot-size: 20px;
  --macOS-nav-gap: 3px;
  --macOS-nav-margin-x: 0.5rem;

}

* {
  --header-height: 41px !important;
}

.titlebar-button-container.mod-right {
  background-color: transparent !important;
  width: fit-content;
  align-items: center;
  gap: var(--macOS-nav-gap);
  padding: 0 var(--macOS-nav-margin-x);

  .titlebar-button.mod-minimize,
  .titlebar-button.mod-maximize,
  .titlebar-button.mod-close {
    color: transparent;
    display: grid;
    place-items: center;
    position: relative;
    padding: 0;
    width: var(--macOS-nav-dot-size) !important;
    aspect-ratio: 1/1;
    border-radius: var(--tab-radius);

    &::after {
      content: "";
      position: absolute;
      width: 12px;
      aspect-ratio: 1/1;
      border-radius: 50%;
      background-color: var(--macOS-nav-dot-color);
    }
  }

  .titlebar-button.mod-minimize {
    order: 2;
    --macOS-nav-dot-color: #edbc65;
  }

  .titlebar-button.mod-maximize {
    order: 3;
    --macOS-nav-dot-color: #72da7c;
  }

  .titlebar-button.mod-close {
    order: 1;
    --macOS-nav-dot-color: #df5252;
    --background-modifier-error: var(--background-modifier-hover);
    /* Disable the background turning red on hover */
  }
}

/* Positioning buttons into the top left. Hacky solution and may cause issues. Tested on desktop/default theme with default sizes only. Works by hiding some elements and shifting things around with margins (translate and padding cause issues). Borders are removed from some elements and added to others to recreate the default theme look. */

/* Move Minimize/Maximize/Close to top left. */
.titlebar-button-container.mod-right {
  left: 0;
  border-bottom: var(--divider-width) solid var(--divider-color);
  background: var(--titlebar-background) !important;
}

/* Shift the the sidebar toggle button. Note that this button fills the height of the entire nav bar, it's not just the icon. */
.side-dock-ribbon .sidebar-toggle-button {
  margin-left: calc(var(--macOS-nav-dot-size) * 3 + var(--macOS-nav-gap) * 2 + var(--macOS-nav-margin-x) + 8px);
  border-bottom: var(--divider-width) solid var(--divider-color);
  background: var(--titlebar-background) !important;
}

/* Make the sidebar toggle button also change background color when the window is focused */
body.is-focused .side-dock-ribbon .sidebar-toggle-button {
  --titlebar-background: var(--titlebar-background-focused);
}

.workspace-tab-header-container {
  /* A bit hacky, can be refactored into removing the border off the outer element and adding it to an inner element instead. */
  margin-top: -1px;
  padding-top: 1px;
  border-bottom: var(--divider-width) solid var(--divider-color);

  &::before {
    display: none !important;
  }
}

/* Slide the tabs over when sidebar is collapsed to make space for new buttons + shifted sidebar toggle button */
.is-collapsed~.mod-root .workspace-tab-header-container {
  margin-left: calc(var(--macOS-nav-dot-size) * 3 + var(--macOS-nav-gap) * 2 + var(--macOS-nav-margin-x)) !important;
}

/* Shift the Files/Search/Bookmarks */
.mod-sidedock.mod-left-split .workspace-tab-header-container {
  margin-left: calc(var(--macOS-nav-dot-size) * 3 + var(--macOS-nav-gap) * 2 + var(--macOS-nav-margin-x) + 8px) !important;
}

/* Adjust padding to fill the space that was made by moving the buttons to the left */
.workspace-tab-header-container {
  padding-right: var(--size-4-2) !important;

  /* Remove the top right corner which prevented dragging at the Windows Minimize/Maximize/Close buttons */
  &::after {
    display: none !important;
  }
}

/* Remove top left corner section making the buttons unclickable. Note that you will not be able to drag the window from the taskbar here. */
.side-dock-ribbon::before {
  display: none !important;
}

/* Since we hid .side-dock-ribbon::before, there is dark space in the top left corner. By swapping the ribbon's margin with padding, we can fill that dark space to match the ribbon color. */
.workspace-ribbon {
  /* 8px is the top value of --ribbon-padding */
  margin-top: 0 !important;
  padding-top: calc(var(--header-height) + 8px - 1px) !important;
}

/* Note title offset */
.workspace-tab-container .workspace-leaf-content .view-header .view-header-title-container {
  margin-top: -1px;
}
```
