---
author: rushi
source:
cover: "[[img-custom checkbox - task priorities.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Custom checkbox - task priorities

![](../attachments/img-custom%20checkbox%20-%20task%20priorities.webp)

## Snippet

```css
.HyperMD-list-line:has(.cm-tag-p1) .task-list-label {
  --checkbox-border-color: red;
}

.task-list-item:has([href="#p1"]) {
  --checkbox-border-color: red;
}

.HyperMD-list-line:has(.cm-tag-p2) .task-list-label {
  --checkbox-border-color: gold;
}

.task-list-item:has([href="#p2"]) {
  --checkbox-border-color: gold;
}

.HyperMD-list-line:has(.cm-tag-p3) .task-list-label {
  --checkbox-border-color: #1895f5;
}

.task-list-item:has([href="#p3"]) {
  --checkbox-border-color: #1895f5;
}
```

## How to use

```md
- [ ] High priority #p1
- [ ] Medium priority #p2
- [ ] Low priority #p3
```