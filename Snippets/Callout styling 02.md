↪[Collection](Collection.md)

# Callout Styling 02

---

- author:: kneecaps
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1053024490843557958

---

> _I've modified the original code a bit to get this look_

cover:: ![](https://i.imgur.com/izbQq7Q.png)

```css
.callout::after {
  content: "";
  width: 48px;
  height: 15px;
  border-radius: 8px;
  position: absolute;
  display: inline-block;
  background: rgb(var(--callout-color));
  margin-top: 0.3%;
  margin-left: auto;
  border: var(--border-lowOp);
  box-shadow: var(--sbs);
}

.callout {
  background: transparent;
}

body {
  --callout-border-width: 2px;
  --callout-border-opacity: 1;
}
```

---

## Original code

```css
.callout::after {
  content: "";
  width: 48px;
  height: 12px;
  border-radius: 8px;
  position: absolute;
  display: inline-block;
  background: rgb(var(--callout-color));
  margin-top: 0.3%;
  margin-left: auto;
  border: var(--border-lowOp);
  box-shadow: var(--sbs);
}
```
