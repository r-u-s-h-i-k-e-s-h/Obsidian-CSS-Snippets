---
author: The Useful Walrus
source: https://discord.com/channels/686053708261228577/702656734631821413/1144209029464342538
cover: "[[gif-properties - show on hover.gif]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Properties - show on hover

![](../attachments/gif-properties%20-%20show%20on%20hover.gif)

## Snippet

```css
/*
author: The Useful Walrus
source: https://discord.com/channels/686053708261228577/702656734631821413/1144209029464342538
*/

.metadata-properties-title {
  transition: 500ms;
  opacity: 0.2;
  pointer-events: none;
}

.metadata-container:hover .metadata-properties-title {
  opacity: 1;
  color: var(--text-accent);
  pointer-events: auto;
}

.metadata-content {
  transition: 200ms cubic-bezier(0.25, 1, 0.5, 1);
  opacity: 0;
  height: 0;
  margin-bottom: -1.8em;
  pointer-events: none;
}

.metadata-container:hover .metadata-content {
  opacity: 1;
  height: auto;
  margin-bottom: 0.5em;
  pointer-events: auto;
}
```
