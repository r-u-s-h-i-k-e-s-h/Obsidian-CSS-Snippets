---
author: BunkerD
source: https://forum.obsidian.md/t/a-callout-for-a-folder-structure/61366
cover: "[[img-callout styling - folder structure.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - folder structure

![](../attachments/img-callout%20styling%20-%20folder%20structure.webp)

## Snippet

```css
/*
author: BunkerD
source: https://forum.obsidian.md/t/a-callout-for-a-folder-structure/61366
*/

.callout[data-callout="folder" i] {
  --list-indent: 0em;
  --indentation-guide-color: transparent;
  overflow: scroll;
}

.callout[data-callout="folder" i] .list-bullet {
  display: none;
}

.callout[data-callout="folder" i] ul {
  -webkit-margin-after: 0;
  margin-block-end: 0;
}

.callout[data-callout="folder" i] li {
  --list-indent: 1.5em;
  list-style-type: none;
  font-family: var(--font-monospace);
  white-space: nowrap;
}

.callout[data-callout="folder" i] li li {
  position: relative;
  box-sizing: border-box;
}

.callout[data-callout="folder" i] li li::before,
.callout[data-callout="folder" i] li li::after {
  content: "";
  position: absolute;
  left: -1em;
  background: var(--list-marker-color);
}

.callout[data-callout="folder" i] li li::before {
  top: 0.85em;
  width: 10px;
  height: 1.5px;
  margin: auto;
}

.callout[data-callout="folder" i] li li::after {
  top: 0;
  bottom: 0;
  width: 1.5px;
  height: 100%;
}

.callout[data-callout="folder" i] li li:last-child::after {
  height: 0.85em;
}

.callout[data-callout="folder" i] li .list-collapse-indicator {
  position: absolute;
  left: -2em;
  margin: 0;
}

.callout[data-callout="folder" i] li em {
  opacity: 0.5;
  font-family: var(--font-text);
}

.callout[data-callout="folder" i] li code {
  font-size: 1em;
  font-family: var(--font-monospace);
  font-style: normal !important;
  background: none;
  white-space: pre;
  margin: 0;
  padding: 0;
}

.callout[data-callout="folder" i] li mark {
  font-style: italic;
  color: #d3a3e5;
}

.callout[data-callout="folder" i] .callout-content {
  overflow-x: visible;
}
```

## How to use

```md
> [!folder] folder
>
> - 📁 Folder _`           `← root folder_
>   - 📄 Item 1 _`         `← some item in the folder_
>   - 📁 Subfolder 1 _`    `← another folder_
>     - 📄 Subitem 1-1
>     - 📄 Subitem 1-2
>   - 📁 Subfolder 2
>     - 📄 Subitem 2-1
>     - 📄 Subitem 2-2
>     - 📁 Subsubfolder
>       - 📄 ==Name==.jpg _`   `… Some variable name?_
>       - …
```
