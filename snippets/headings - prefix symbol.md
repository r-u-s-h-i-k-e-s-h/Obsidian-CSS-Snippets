---
author: rushi
source:
cover: "[[img-headings - prefix symbol.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Headings - prefix symbol

> You can change `§` with something else

![](../attachments/img-headings%20-%20prefix%20symbol.webp)

## Snippet

```css
:is(h1,
  h2,
  h3,
  h4,
  h5,
  h6,
  .HyperMD-header-1,
  .HyperMD-header-2,
  .HyperMD-header-3,
  .HyperMD-header-4,
  .HyperMD-header-5,
  .HyperMD-header-6)::before {
  content: "§ ";
  font-size: 0.7em;
  vertical-align: middle;
  color: var(--text-accent);
  font-weight: 500;
}
```
