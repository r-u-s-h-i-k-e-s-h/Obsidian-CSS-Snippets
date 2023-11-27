↪[Collection](Collection.md)

# Author callout

---

- author:: rushi
- reference:: https://discord.com/channels/686053708261228577/702656734631821413/1096863934100807701

---

cover:: ![](https://i.imgur.com/2PuEAwx.png)

```css
.callout[data-callout="author"] {
  display: flex;
  flex-direction: column-reverse;
  --callout-icon: user;
  --callout-color: transparent;
  box-shadow: rgba(0, 0, 0, 0.1) 0px 10px 50px;
  border-left: solid;
}

.callout[data-callout="author"] > .callout-title {
  display: flex;
  justify-content: flex-end;
  padding-right: 8px;
  font-style: italic;
}

.callout[data-callout="author"] .callout-content p {
  margin-top: 0;
}
```
