---
author: kneecaps
source:
cover: "[[img-explorer styling - new note button.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Explorer styling - new note button

> Extracted form [Origami Theme](https://github.com/7368697661/Origami) of **kneecaps**

![](../attachments/img-explorer%20styling%20-%20new%20note%20button.webp)

## Snippet

```css
/*
MIT License

Copyright (c) 2022 kneecaps

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
*/

.clickable-icon[aria-label="New note"] {
  padding: 0px 8px 0px 4px;
  border: 1px solid var(--titlebar-border-color);
}

.clickable-icon[aria-label="New note"]::before {
  content: "New Note";
  padding: 0px 8px;
}
```
