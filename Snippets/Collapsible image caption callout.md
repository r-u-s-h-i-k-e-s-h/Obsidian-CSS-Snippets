↪[Collection](Collection.md)

# Collapsible image caption callout

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1134127383872536576

---

cover:: ![](https://i.imgur.com/mquPDHu.gif)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1134127383872536576
*/

/* image caption collapsible callout */
.callout[data-callout="img-caption"] {
  --callout-color: none;
  --callout-icon: none;
  padding: 12px 0px;
}
.callout[data-callout="img-caption"] > .callout-title {
  font-size: 0px;
  justify-content: center;
}
.callout[data-callout="img-caption"]
  > .callout-title
  > :is(.callout-icon, .callout-fold) {
  display: none;
}
.callout[data-callout*="img-caption"] > .callout-content {
  text-align: center;
}
```

---

## How to use

```md
> [!img-caption]- ![[img name.format]]
> Lorem, ipsum dolor sit amet consectetur, adipisicing elit.
```
