↪[Collection](Collection.md)

# Heading indicators 01

---

- author:: rushi
- source::

---

cover:: ![](https://i.imgur.com/AVh7wWL.png)

```css
:is(
    h1,
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
    .HyperMD-header-6
  )::after {
  font-size: 12px;
  padding-left: 3em;
  color: var(--text-accent);
}

/* reading mode */
h1::after {
  content: "...H1";
}
h2::after {
  content: "...H2";
}
h3::after {
  content: "...H3";
}
h4::after {
  content: "...H4";
}
h5::after {
  content: "...H5";
}
h6::after {
  content: "...H6";
}

/* live preview */
.HyperMD-header-1:not(.cm-active)::after {
  content: "...H1";
}
.HyperMD-header-2:not(.cm-active)::after {
  content: "...H2";
}
.HyperMD-header-3:not(.cm-active)::after {
  content: "...H3";
}
.HyperMD-header-4:not(.cm-active)::after {
  content: "...H4";
}
.HyperMD-header-5:not(.cm-active)::after {
  content: "...H5";
}
.HyperMD-header-6:not(.cm-active)::after {
  content: "...H6";
}
```
