↪[Collection](Collection.md)

# Table styling - Left column header

---

- author:: zamsyt
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1076475103006687232

---

> _Only works in reading mode_

cover:: ![](https://i.imgur.com/yVG3f3o.png)

```css
/*
author: zamsyt
source: https://discord.com/channels/686053708261228577/702656734631821413/1076475103006687232
*/

:is(.cm-table-widget, .markdown-preview-section > div):has(+ * .left-thead) th {
  font-weight: unset;
}
:is(.cm-table-widget, .markdown-preview-section > div):has(+ * .left-thead)
  > table
  > *
  > tr
  > :first-child {
  font-weight: var(--table-header-weight);
  background-color: var(--background-secondary);
}
```

---

## How to use

```md
| Header 1 | Header 2 | Header 3 | Header 4 |
| :------: | :------: | :------: | :------: |
| Value A  | Value B  | Value C  | Value D  |
| Value E  | Value F  | Value G  | Value H  |
| Value I  | Value J  | Value K  | Value L  |

<b class="left-thead"></b>
```

> [!warning] Remember to put `<b class="left-thead"></b>` at the bottom of the table
