---
author: Kapirklaa
source: https://discord.com/channels/686053708261228577/702656734631821413/1285396797090697289
cover: "[[img-callout styling - bullet icon.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - bullet icon

![](../attachments/img-callout%20styling%20-%20bullet%20icon.webp)

## Snippet

```css
/* 
author: Kapirklaa
source: https://discord.com/channels/686053708261228577/702656734631821413/1285396797090697289
*/

.markdown-source-view.mod-cm6 .cm-callout,
.callout {
  --callout-icon-size: 14px;
  --callout-icon-bullet-size: calc(var(--callout-icon-size) + var(--size-4-3));
}

.callout {
  --callout-radius: var(--radius-m);
  --callout-border-width: 4px;
  --callout-border-opacity: 1;

  border-top: none;
  border-right: none;
  border-bottom: none;

  position: relative;
  overflow: visible;
  box-shadow: 0 5px 15px rgba(0, 0, 0, 0.2);
  min-height: calc(var(--icon-bullet-size) + 2 * var(--size-4-3));

  .callout-icon {
    --icon-size: var(--callout-icon-size);
    position: absolute;
    top: calc(var(--size-4-3) * 0.75);
    left: calc(-0.5 * var(--callout-icon-bullet-size) - 0.5 * var(--callout-border-width));
    gap: 0;
    background-color: rgb(var(--callout-color));
    border-radius: 50%;
    width: var(--callout-icon-bullet-size);
    height: var(--callout-icon-bullet-size);
    justify-content: center;
    align-items: center;
  }

  .callout-icon svg {
    color: white;
  }
}

.markdown-preview-view .callout {
  margin-left: calc(0.5 * var(--callout-icon-bullet-size));
}

.markdown-source-view.mod-cm6 .cm-callout {
  padding-left: calc(0.5 * var(--callout-icon-bullet-size));
}

.markdown-source-view.mod-cm6 .cm-content>.cm-callout[contenteditable=false] {
  contain: unset !important;
}
```
