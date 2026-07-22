---
author:
  - kneecaps
source: https://discord.com/channels/686053708261228577/702656734631821413/1053024490843557958
cover: "[[img-callout styling - bottom pill.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - bottom pill

![](../attachments/img-callout%20styling%20-%20bottom%20pill.webp)

## Snippet

```css
/*
author: kneecaps
source: https://discord.com/channels/686053708261228577/702656734631821413/1053024490843557958
*/

.callout::after {
  content: "";
  width: 48px;
  height: 12px;
  border-radius: 8px;
  position: absolute;
  display: inline-block;
  background: rgb(var(--callout-color));
  margin-top: 0.3%;
  margin-left: auto;
  border: var(--border-lowOp);
  box-shadow: var(--sbs);
}
```
