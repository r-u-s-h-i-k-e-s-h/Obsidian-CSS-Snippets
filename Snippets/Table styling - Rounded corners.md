↪[Collection](Collection.md)

# Table styling - Rounded corners

---

- author:: FireIsGood
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1112164539975340032

---

cover:: ![](https://i.imgur.com/OEAPHo8.png)

```css
/*
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1112164539975340032
*/

:root table {
  border-collapse: separate;
  border-spacing: 0;
}
th:first-of-type {
  border-top-left-radius: 8px;
}
th:last-of-type {
  border-top-right-radius: 8px;
}
tr:last-of-type td:first-of-type {
  border-bottom-left-radius: 8px;
}
tr:last-of-type td:last-of-type {
  border-bottom-right-radius: 8px;
}

:root :is(td, th) {
  border-width: 0 var(--table-border-width) var(--table-border-width) 0;
}
```
