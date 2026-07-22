---
author: zamsyt
source: https://discord.com/channels/686053708261228577/702656734631821413/1076475103006687232
cover: "[[img-table styling - first column header.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Table styling - first column header

> Only works in reading mode

![](../attachments/img-table%20styling%20-%20first%20column%20header.webp)

## Snippet

```css
/*
author: zamsyt
source: https://discord.com/channels/686053708261228577/702656734631821413/1076475103006687232
*/

:is(.cm-table-widget, .markdown-preview-section > div):has(+ * .left-thead) th {
  font-weight: unset;
}

:is(.cm-table-widget, .markdown-preview-section > div):has(+ * .left-thead)>table>*>tr> :first-child {
  font-weight: var(--table-header-weight);
  background-color: var(--background-secondary);
}
```

## How to use

```md
| Header 1 | Header 2 | Header 3 | Header 4 |
| :------: | :------: | :------: | :------: |
| Value A  | Value B  | Value C  | Value D  |
| Value E  | Value F  | Value G  | Value H  |
| Value I  | Value J  | Value K  | Value L  |
| Value M  | Value N  | Value O  | Value P  |

<b class="left-thead"></b>
```

