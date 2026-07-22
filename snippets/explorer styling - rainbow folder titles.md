---
author:
  - sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1163095446919585843
cover: "[[img-explorer styling - rainbow folder titles.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Explorer styling - rainbow folder titles

![](../attachments/img-explorer%20styling%20-%20rainbow%20folder%20titles.webp)

## Snippet

```css
/*
Original Author: sailKite
Source: https://discord.com/channels/686053708261228577/702656734631821413/1163095446919585843
Modified By: rushi

Note: added light/dark support
*/

.nav-files-container>div>.nav-folder {
  --nav-item-color: var(--folder-color);

  &:hover {
    filter: brightness(0.9);
  }

  .theme-dark & {
    &:nth-child(11n + 2) {
      --folder-color: rgb(243, 139, 168);
    }

    &:nth-child(11n + 3) {
      --folder-color: rgb(235, 160, 172);
    }

    &:nth-child(11n + 4) {
      --folder-color: rgb(250, 179, 135);
    }

    &:nth-child(11n + 5) {
      --folder-color: rgb(249, 226, 175);
    }

    &:nth-child(11n + 6) {
      --folder-color: rgb(166, 227, 161);
    }

    &:nth-child(11n + 7) {
      --folder-color: rgb(148, 226, 213);
    }

    &:nth-child(11n + 8) {
      --folder-color: rgb(137, 220, 235);
    }

    &:nth-child(11n + 9) {
      --folder-color: rgb(116, 199, 236);
    }

    &:nth-child(11n + 10) {
      --folder-color: rgb(135, 176, 249);
    }

    &:nth-child(11n + 11) {
      --folder-color: rgb(180, 190, 254);
    }

    &:nth-child(11n + 12) {
      --folder-color: rgb(203, 166, 247);
    }
  }

  .theme-light & {
    &:nth-child(11n + 2) {
      --folder-color: rgb(210, 15, 57);
    }

    &:nth-child(11n + 3) {
      --folder-color: rgb(230, 69, 83);
    }

    &:nth-child(11n + 4) {
      --folder-color: rgb(254, 100, 11);
    }

    &:nth-child(11n + 5) {
      --folder-color: rgb(223, 142, 29);
    }

    &:nth-child(11n + 6) {
      --folder-color: rgb(64, 160, 43);
    }

    &:nth-child(11n + 7) {
      --folder-color: rgb(23, 146, 153);
    }

    &:nth-child(11n + 8) {
      --folder-color: rgb(4, 165, 229);
    }

    &:nth-child(11n + 9) {
      --folder-color: rgb(32, 159, 181);
    }

    &:nth-child(11n + 10) {
      --folder-color: rgb(30, 102, 245);
    }

    &:nth-child(11n + 11) {
      --folder-color: rgb(114, 135, 253);
    }

    &:nth-child(11n + 12) {
      --folder-color: rgb(136, 57, 239);
    }
  }
}
```
