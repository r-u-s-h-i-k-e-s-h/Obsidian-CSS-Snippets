↪[Collection](Collection.md)

# Properties into two columns

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1155496243691266158

---

cover:: ![](https://i.imgur.com/8zFYyGV.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1155496243691266158
*/

[data-type="markdown"] .metadata-properties {
  display: grid;
  grid: auto-flow / 50% 50%;
  gap: 3px 0px;
}

[data-type="markdown"] .metadata-properties .metadata-property-value {
  align-items: start;
}

body {
  --metadata-label-width: 5em;
}
```
