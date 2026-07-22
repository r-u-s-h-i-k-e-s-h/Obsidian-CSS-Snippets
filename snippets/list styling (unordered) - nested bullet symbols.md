---
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1215687753489055785
cover: "[[img-list styling (unordered) - nested bullet symbols.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# List styling (unordered) - nested bullet symbols

![](../attachments/img-list%20styling%20(unordered)%20-%20nested%20bullet%20symbols.webp)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1215687753489055785
*/

/* custom unordered list basic properties */
body {
  --ul-01-punct: "◇";
  --ul-02-punct: "⨯";
  --ul-03-punct: "♥";
  --ul-04-punct: var(--ul-01-punct);
}

/* unordered list rendered counters */
.markdown-rendered ul {
  /* level 1 */
  --list-punct: var(--ul-01-punct);

  /* level 2 */
  &>li>ul {
    --list-punct: var(--ul-02-punct);

    /* level 3 */
    &>li>ul {
      --list-punct: var(--ul-03-punct);

      /* level 4 */
      &>li>ul {
        --list-punct: var(--ul-04-punct);
      }
    }
  }

  &>li>.list-bullet::before {
    color: var(--list-marker-color);
    translate: -50%;
  }

  &>li>.list-bullet::after {
    background-color: transparent;
  }

  :is(&, &:not(li ul))>li>.list-bullet::before {
    content: var(--list-punct) " ";
  }
}

.is-live-preview {

  /* unordered list edit mode counters */
  /* default */
  & .HyperMD-list-line:not(.cm-active)>.cm-formatting-list-ul {
    font-size: 0px;

    &::before {
      content: var(--ul-01-punct) " ";
      font-size: var(--font-text-size);
    }
  }

  /* level 1 */
  & .HyperMD-list-line-1:not(.cm-active)>.cm-formatting-list-ul::before {
    content: var(--ul-01-punct) " ";
  }

  /* level 2 */
  & .HyperMD-list-line-2:not(.cm-active)>.cm-formatting-list-ul::before {
    content: var(--ul-02-punct) " ";
  }

  /* level 3 */
  & .HyperMD-list-line-3:not(.cm-active)>.cm-formatting-list-ul::before {
    content: var(--ul-03-punct) " ";
  }

  /* level 4 */
  & .HyperMD-list-line-4:not(.cm-active)>.cm-formatting-list-ul::before {
    content: var(--ul-04-punct) " ";
  }
}
```
