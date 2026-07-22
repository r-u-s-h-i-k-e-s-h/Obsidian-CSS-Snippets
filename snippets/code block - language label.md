---
author: Kapirklaa
source: https://discord.com/channels/686053708261228577/702656734631821413/1274004487228624986
cover: "[[img-code block - language label.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Code block - language label

![](../attachments/img-code%20block%20-%20language%20label.webp)

## Snippet

```css
/*
author: Kapirklaa
source: https://discord.com/channels/686053708261228577/702656734631821413/1274004487228624986
*/

.markdown-rendered pre {
  padding-top: calc(var(--font-ui-smaller) + 6px * 2 + 6px * 2);

  &::before {
    content: attr(class);
    position: absolute;
    right: 50px;
    /* change that to adapt the space */
    top: 12px;
    font-size: var(--font-ui-smaller);
  }
}
```
