---
author: ryanjamurphy
source: https://discord.com/channels/686053708261228577/1050087185602334833/1256254611837157437
cover: "[[img-canvas styling - no border background when it has callout.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Canvas styling - no border background when it has callout

![](../attachments/img-canvas%20styling%20-%20no%20border%20background%20when%20it%20has%20callout.webp)

## Snippet

```css
.canvas-node-container:has(div.callout) {
  background-color: transparent;
  border: 0;
  box-shadow: none;
}
```
