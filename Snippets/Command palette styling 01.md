↪[Collection](Collection.md)

# Command palette styling 01

---

- author:: rushi
- source::

---

cover:: ![](https://i.imgur.com/1gctisH.gif)

```css
.prompt {
  border: solid var(--text-accent);
  opacity: 0.9;
}

.suggestion-highlight {
  text-decoration: none;
  color: var(--text-accent);
}

.suggestion-item.is-selected {
  border: solid var(--text-accent);
  border-radius: 14px;
}

.suggestion-hotkey {
  background-color: var(--text-accent);
  color: black;
  border-radius: 10px;
  font-weight: 500;
}

.prompt-instruction {
  font-weight: 500;
}

.prompt-instruction-command {
  background-color: rgb(250, 252, 255, 0.5);
  color: black;
  border-radius: 10px;
  padding: 0 3px 0 3px;
}
```
