↪[Collection](Collection.md)

# Celtic inline title styling

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1163153997465653370

---

cover:: ![](https://i.imgur.com/cMSMue3.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1163153997465653370
*/

.inline-title {
  display: flex;
  justify-content: center;
  gap: 2.5%;
  align-items: center;

  &::before,
  &::after {
    content: "";
    background-image: url("https://media.discordapp.net/attachments/702656734631821413/1163152299464605909/Obsiidan_border_detail.png?ex=653e88fe&is=652c13fe&hm=0213a2468a424a48e898c3a02a621c9e0a102b902fd8fb6e48fa8bd43d8c1cd3&=&width=300&height=147");
    background-size: contain;
    background-repeat: no-repeat;
    background-position: center;
    flex: 0 0 5em;
    aspect-ratio: 1;
  }

  &::after {
    scale: -1 1;
  }
}
```
