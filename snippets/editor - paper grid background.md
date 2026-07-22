---
author: Melvin
source: https://discord.com/channels/686053708261228577/702656734631821413/1000912780611829870
cover: "[[img-editor - paper grid background.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Editor - paper grid background

![](../attachments/img-editor%20-%20paper%20grid%20background.webp)

## Snippet

```css
/*
author: Melvin
source: https://discord.com/channels/686053708261228577/702656734631821413/1000912780611829870
*/

.workspace-leaf-content[data-type=markdown] .view-content {
  background-image: repeating-linear-gradient(to right, var(--background-secondary), var(--background-secondary) 1px, transparent 1px, transparent 20px), repeating-linear-gradient(to top, var(--background-secondary), var(--background-secondary) 1px, transparent 1px, transparent 20px);
}
```
