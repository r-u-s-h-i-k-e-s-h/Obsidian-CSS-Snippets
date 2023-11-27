↪[Collection](Collection.md)

# Link styling 01

---

- author:: rushi
- source::

---

> _Inspired from [Origami theme](https://github.com/7368697661/Origami)_ of **kneecaps**.

cover:: ![](https://i.imgur.com/4Twe0hL.gif)

```css
.markdown-source-view.mod-cm6 .is-unresolved .cm-underline,
.markdown-source-view.mod-cm6 .cm-underline.is-unresolved,
.markdown-source-view.mod-cm6 .cm-underline {
  text-decoration-line: underline;
  text-decoration-thickness: 2px;
  color: var(--text-normal);
  text-decoration-color: var(--color-accent);
  text-decoration-skip-ink: none;
  font-weight: 600;
}

.markdown-rendered .internal-link {
  text-decoration-line: underline;
  text-decoration-thickness: 2px;
  color: var(--text-normal);
  text-decoration-color: var(--color-accent);
  text-decoration-skip-ink: none;
  font-weight: 600;
}
.markdown-rendered .internal-link:hover {
  text-decoration: none;
  color: var(--text-accent);
  font-weight: 600;
}

.external-link {
  text-decoration-line: underline;
  text-decoration-thickness: 2px;
  color: var(--text-normal);
  text-decoration-color: var(--color-accent);
  text-decoration-skip-ink: none;
  font-weight: 600;
}

.external-link:hover {
  text-decoration: none;
  color: var(--text-accent);
  font-weight: 600;
}
```
