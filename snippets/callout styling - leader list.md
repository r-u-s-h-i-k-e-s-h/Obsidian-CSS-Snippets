---
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1148625898074017863
cover: "[[img-callout styling - leader list.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - leader list

![](../attachments/img-callout%20styling%20-%20leader%20list.webp)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1148625898074017863
*/

/* goofy attempt at dot leaders */
.callout[data-callout="leader-list"] {
  --callout-color: unset;
  --callout-icon: unset;
  --callout-blend-mode: normal;
  padding: unset;
  margin: unset;
}

.callout[data-callout="leader-list"]>.callout-title {
  display: none;
}

.callout[data-callout="leader-list"]>.callout-content {
  --gap: var(--size-2-2);
  display: grid;
  grid-template-columns: 1fr auto;
  row-gap: var(--gap);
}

.callout[data-callout="leader-list"]>.callout-content>p {
  display: grid;
  grid-template-columns: auto 1fr;
  margin: unset;
}

.callout[data-callout="leader-list"]>.callout-content>p::after {
  content: " ";
  background-image: radial-gradient(circle,
      currentColor 0px 0.1em,
      transparent 0.1em);
  background-size: 0.5em 1em;
  background-position: bottom right;
  background-repeat: repeat-x;
}

.callout[data-callout="leader-list"]>.callout-content>blockquote {
  padding: unset;
  margin: unset;
  border: unset;
  align-self: center;
  text-align: end;
}
```

## How to use

```md
> [!leader-list] none
>
> Chapter 01
> > 09
>
> Chapter 02
> > 10
>
> Chapter 03
> > 11
>
> Chapter 04
> > 19
```
