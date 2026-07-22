---
author: rushi
source:
cover: "[[img-callout styling - without icon.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - without icon

![](../attachments/img-callout%20styling%20-%20without%20icon.webp)

## Snippet

```css
.callout:is([data-callout-metadata="noicon"]) .callout-icon {
  display: none;
}
```

## How to use

```md
> [!done|noicon] Title
> Lorem, ipsum dolor sit amet consectetur, adipisicing elit.
```
