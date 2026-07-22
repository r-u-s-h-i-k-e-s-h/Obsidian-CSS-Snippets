---
author: rushi
source:
cover: "[[img-headings - indicators trailing.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Headings - indicators trailing

![](../attachments/img-headings%20-%20indicators%20trailing.webp)

## Snippet

```css
:is(h1, h2, h3, h4, h5, h6,
  .HyperMD-header-1, .HyperMD-header-2, .HyperMD-header-3,
  .HyperMD-header-4, .HyperMD-header-5, .HyperMD-header-6)::after {
  font-size: 12px;
  color: var(--text-accent);
  float: right;
  font-weight: normal;
}

h1::after {
  content: "H1";
}

h2::after {
  content: "H2";
}

h3::after {
  content: "H3";
}

h4::after {
  content: "H4";
}

h5::after {
  content: "H5";
}

h6::after {
  content: "H6";
}

.HyperMD-header-1:not(.cm-active)::after {
  content: "H1";
}

.HyperMD-header-2:not(.cm-active)::after {
  content: "H2";
}

.HyperMD-header-3:not(.cm-active)::after {
  content: "H3";
}

.HyperMD-header-4:not(.cm-active)::after {
  content: "H4";
}

.HyperMD-header-5:not(.cm-active)::after {
  content: "H5";
}

.HyperMD-header-6:not(.cm-active)::after {
  content: "H6";
}
```
