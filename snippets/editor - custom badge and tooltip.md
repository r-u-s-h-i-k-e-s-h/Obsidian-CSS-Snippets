---
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1204635191986094141
cover: "[[img-editor - custom badge and tooltip.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Editor - custom badge and tooltip

![](../attachments/img-editor%20-%20custom%20badge%20and%20tooltip.webp)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1204635191986094141
*/

.badge-one {
  position: relative;
  display: inline-block;
  width: 20px;
  height: 20px;
  margin-right: 0.5ch;
  border-radius: 4px;
  vertical-align: text-top;
  background-image: url('data:image/svg+xml,<svg xmlns="http://www.w3.org/2000/svg" width="100%" height="100%" viewBox="0 0 24 24" fill="none" stroke="rgb(233, 151, 63)" stroke-width="2" stroke-linecap="round" stroke-linejoin="round" class="lucide lucide-shield-alert"><path d="M12 22s8-4 8-10V5l-8-3-8 3v7c0 6 8 10 8 10"/><path d="M12 8v4"/><path d="M12 16h.01"/></svg>');
}

.badge-one:hover::after {
  content: "Requires a login.";
  position: absolute;
  z-index: 1;
  bottom: 100%;
  left: 100%;
  padding: var(--size-4-1);
  border: 2px solid var(--color-orange);
  border-radius: 4px;
  background-color: var(--background-primary);
  white-space: nowrap;
}
```

## How to use

```md
<span class="badge-one"></span> Lorem, ipsum dolor sit amet consectetur, adipisicing elit
```