↪[Collection](Collection.md)

# Code block styling 01

---

- author:: kneecaps
- source::

---

> _Extracted from [Origami theme](https://github.com/7368697661/Origami) of_ **kneecaps**.

cover:: ![](https://i.imgur.com/EX3aQgt.png)

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

/* reading mode */
.markdown-rendered pre {
  border: solid var(--color-accent);
  border-radius: var(--radius-m);
  box-shadow: var(--shadow-lm-only);
}

/* live preview */
.cm-s-obsidian div.HyperMD-codeblock-begin-bg {
  background: var(--code-background);
  border-top: solid var(--color-accent);
  /* stylelint-disable-next-line declaration-no-important */
  border-top-right-radius: 8px !important;
  /* stylelint-disable-next-line declaration-no-important */
  border-top-left-radius: 8px !important;
  margin-top: 8px;
}

.cm-s-obsidian div.HyperMD-codeblock-end-bg {
  background: var(--code-background);
  border-bottom: solid var(--color-accent);
  border-bottom-right-radius: 8px;
  border-bottom-left-radius: 8px;
}

.cm-s-obsidian div.HyperMD-codeblock-bg {
  border-right: solid var(--color-accent);
  border-left: solid var(--color-accent);
}
```
