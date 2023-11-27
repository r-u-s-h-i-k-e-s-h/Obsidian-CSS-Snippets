↪[Collection](Collection.md)

# Equally spaced dataview columns

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/707816848615407697/1154034583478751282

---

cover:: ![](https://i.imgur.com/fU7LRj3.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/707816848615407697/1154034583478751282
*/

.dv-equal-columns .dataview.table-view-table tr > * {
  width: calc(100% / var(--dv-col-count));
}
.dv-equal-columns .dataview.table-view-table {
  :has(> tr > :nth-child(2)) {
    --dv-col-count: 2;
  }
  :has(> tr > :nth-child(3)) {
    --dv-col-count: 3;
  }
  :has(> tr > :nth-child(4)) {
    --dv-col-count: 4;
  }
  :has(> tr > :nth-child(5)) {
    --dv-col-count: 5;
  }
  :has(> tr > :nth-child(6)) {
    --dv-col-count: 6;
  }
}
```

---

## How to use

```md
---
cssclasses:
  - dv-equal-columns
---
```
