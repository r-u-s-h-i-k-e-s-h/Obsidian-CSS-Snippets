↪[Collection](Collection.md)

# Callout styling - Minimal callout

---

- author:: rushi
- source::

---

cover:: ![](https://i.imgur.com/nmyuR4y.png)

```css
.callout[data-callout="m-callout"] {
  --callout-color: transparent;
  border: none;
  padding: 0;
}

.callout[data-callout="m-callout"] .callout-title {
  display: none;
  padding: 0;
}

.callout[data-callout="m-callout"] .callout-content {
  font-size: 85%;
  text-align: center;
}

.callout[data-callout="m-callout"] .callout-content::after {
  content: "--- ♪ ♪ ♪ ---";
  color: var(--text-accent);
}
```

---

## How to use

```md
> [!m-callout] Title
> Lorem ipsum dolor sit amet consectetur adipisicing elit. Minus assumenda iusto sint officia quas distinctio doloribus harum optio commodi eum!
```
