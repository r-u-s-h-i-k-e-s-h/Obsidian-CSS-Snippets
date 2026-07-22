---
author: pseudometa
source: https://discord.com/channels/686053708261228577/702656734631821413/893816224247586868
cover: "[[gif-text styling - spoiler text.gif]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Text styling - spoiler text

> Only works in reading mode

![](../attachments/gif-text%20styling%20-%20spoiler%20text.gif)

## Snippet

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

div:not(.CodeMirror-activeline)>.CodeMirror-line .cm-em.cm-strikethrough,
em>del {
  font-style: initial;
  text-decoration: unset;
  background-color: var(--spoiler-bg);
  color: var(--spoiler-bg);
}

.CodeMirror-activeline>.CodeMirror-line .cm-em.cm-strikethrough,
em>del:hover,
.cm-em.cm-strikethrough:hover {
  background-color: var(--background-secondary-alt) !important;
}
```

## How to use

```md
_~~your text here~~_
```
