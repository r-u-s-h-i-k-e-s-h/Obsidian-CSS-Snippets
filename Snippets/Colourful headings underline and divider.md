↪[Collection](Collection.md)

# Colourful headings underline and divider

---

- author:: relkion
- source:: https://discord.com/channels/686053708261228577/744933215063638183/1006815302866186260

---

cover:: ![](https://i.imgur.com/P1V3vIJ.png)

```css
/*
author: relkion
source: https://discord.com/channels/686053708261228577/744933215063638183/1006815302866186260
*/

/*--colorful heading underline for headings and hr--*/

h1::after,
.HyperMD-header-1::after,
h2::after,
.HyperMD-header-2::after,
h3::after,
.HyperMD-header-3::after,
h4::after,
.HyperMD-header-4::after,
h5::after,
.HyperMD-header-5::after,
h6::after,
.HyperMD-header-6::after,
.markdown-preview-view hr,
.hr.cm-line,
.HyperMD-hr-bg {
  background: linear-gradient(
    90deg,
    rgba(194, 24, 91, 0.8) 10%,
    rgba(137, 46, 127, 0.8) 0 20%,
    rgba(79, 67, 163, 0.8) 0 30%,
    rgba(34, 103, 163, 0.8) 0 40%,
    rgba(0, 151, 167, 0.8) 0 50%,
    rgba(82, 173, 90, 0.8) 0 60%,
    rgba(166, 172, 64, 0.8) 0 70%,
    rgba(249, 171, 37, 0.8) 0 80%,
    rgba(230, 109, 42, 0.8) 0 90%,
    rgba(211, 47, 47, 0.8) 0
  );
}

/*--center h1--*/
h1,
.HyperMD-header-1 {
  text-align: center;
}

h1::after,
.HyperMD-header-1::after,
h2::after,
.HyperMD-header-2::after,
h3::after,
.HyperMD-header-3::after,
h4::after,
.HyperMD-header-4::after,
h5::after,
.HyperMD-header-5::after,
h6::after,
.HyperMD-header-6::after {
  margin-top: 0.2em;
  content: "";
  width: auto !important;
  display: flex !important;
  height: 0.3em;
  border-radius: 10px;
}

/*--Taken from ITS: Horizontal Linebreak, HR--*/
.markdown-source-view.mod-cm6 .cm-content :is(.hr, .HyperMD-hr) {
  contain: style !important;
}

.markdown-preview-view hr,
.hr.cm-line,
.HyperMD-hr-bg {
  margin-block-start: 2em;
  margin-block-end: 2em;
  border: none;
  border-radius: 3px;
  height: 3px;
}

.hr.cm-line hr {
  border: 0;
}

/*Stylized HR/Horizontal Line*/
.hr.cm-line::after,
.markdown-preview-view hr::after,
div:not(.CodeMirror-activeline) > .HyperMD-hr-bg::after {
  content: "★";
  display: inline-block;
  position: absolute;
  left: 50%;
  font-size: 13px;
  color: var(--text-sub-accent);
  padding: 0 0.5em;
  /*--margin-top might need tweaking if symbol is misaligned--*/
  margin-top: -0.6em;
  /*--set to transparent or delete for clear symbol bg--*/
  background-color: var(--background-primary);
}
```

---

## how to use

```md
# Heading

---
```
