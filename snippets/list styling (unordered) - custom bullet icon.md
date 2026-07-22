---
author:
  - SlRvb
  - kneecaps
source: https://discord.com/channels/686053708261228577/931552763467411487/1022340935721439242
cover: "[[img-list styling (unordered) - custom bullet icon.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# List styling (unordered) - custom bullet icon

![](../attachments/img-list%20styling%20(unordered)%20-%20custom%20bullet%20icon.webp)

## Snippet

```css
/*
author: SlRvb, kneecaps
source: https://discord.com/channels/686053708261228577/931552763467411487/1022340935721439242
*/

.list-bullet.list-bullet.list-bullet:after {
  content: "◈";
  height: unset;
  width: unset;
  background: transparent;
  margin-top: 5px;
  color: var(--text-accent);
}
```
