↪[Collection](Collection.md)

# Text styling - Spoiler text

---

- author:: pseudometa
- source:: https://discord.com/channels/686053708261228577/702656734631821413/893816224247586868

---

> _Only works in reading mode._

cover:: ![](https://i.imgur.com/rd71oCp.gif)

```css
/*
author: pseudometa
source: https://discord.com/channels/686053708261228577/702656734631821413/893816224247586868
*/

/* pseudo(meta) spoiler tags */
/* blacks out non-hovered-nonactive text surrounded in *~~text~~* */
.theme-light {
  --spoiler-bg: #111;
}

.theme-dark {
  --spoiler-bg: #eee;
}

div:not(.CodeMirror-activeline) > .CodeMirror-line .cm-em.cm-strikethrough,
em > del {
  font-style: initial;
  text-decoration: unset;
  background-color: var(--spoiler-bg);
  color: var(--spoiler-bg);
}

.CodeMirror-activeline > .CodeMirror-line .cm-em.cm-strikethrough,
em > del:hover,
.cm-em.cm-strikethrough:hover {
  background-color: var(--background-secondary-alt) !important;
}
```

---

## How to use

```md
_~~your text here~~_
```
