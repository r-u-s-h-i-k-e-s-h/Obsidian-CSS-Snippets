↪[Collection](Collection.md)

# Callout styling - Outlined callout

---

- author:: Kepano, sailKite (extracted by)
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1087513978793635860

---

cover:: ![](https://i.imgur.com/d7Cz7m1.png)

```css
/*
author: Kepano, sailKite (extracted by)
source: https://discord.com/channels/686053708261228577/702656734631821413/1087513978793635860
*/

/* ---------------------------------------------------------------------------

Bordered Callouts from Minimal Theme by @kepano

User interface replacement for Obsidian.

Sponsor my work:
https://www.buymeacoffee.com/kepano

Readme:
https://github.com/kepano/obsidian-minimal

-----------------------------------------------------------------------------

MIT License

Copyright (c) 2020-2023 Stephan Ango (@kepano)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:
The above copyright notice and this permission notice shall be included in 
all copies or substantial portions of the Software.
THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
*/
.callouts-outlined .callout .callout-title {
  background-color: var(--background-primary);
  margin-top: -24px;
  z-index: 200;
  width: fit-content;
  padding: 0 0.5em;
  margin-left: -0.75em;
  letter-spacing: 0.05em;
  font-variant-caps: all-small-caps;
}
.callouts-outlined .callout {
  overflow: visible;
  --callout-border-width: 1px;
  --callout-border-opacity: 0.5;
  --callout-title-size: 0.8em;
  --callout-blend-mode: normal;
  background-color: transparent;
}
.callouts-outlined .cm-embed-block.cm-callout {
  padding-top: 12px;
}
.callouts-outlined .callout-content .callout {
  margin-top: 18px;
}
```

---

## Usage

```md
---
cssclasses:
	- callouts-outlined
---
```
