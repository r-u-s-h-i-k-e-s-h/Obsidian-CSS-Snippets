↪[Collection](Collection.md)

# Tags styling - Target specific tag

---

- author:: rushi
- source::

---

> _Only works in reading mode._

cover:: ![](https://i.imgur.com/HhjZpgh.png)

```css
/* Tags styling - Target specific tag */
.tag[href^="#obsidian"] {
  background-color: rgb(var(--color-obsidian-rgb), 0.1);
  color: var(--obsidian);
  font-weight: bolder;
}

/* Feel free to customize for other tags by modifying the selector and color variables below */

body {
  --color-obsidian-rgb: 233, 49, 71;
  --obsidian: rgb(var(--color-obsidian-rgb));
}
```
