↪[Collection](Collection.md)

# Tooltip styling

---

- author:: kneecaps
- source::

---

> _Extracted form [Origami Theme](https://github.com/7368697661/Origami)_ of **kneecaps**

cover:: ![](https://i.imgur.com/wyGvM7S.png)

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

.tooltip {
  background-color: var(--red);
  color: black;
  word-wrap: break-word;
}
.tooltip .tooltip-arrow {
  border-bottom: 5px solid var(--red);
}
.tooltip.mod-right .tooltip-arrow {
  border-right: 5px solid var(--red);
}
.tooltip.mod-left .tooltip-arrow {
  border-left: 5px solid var(--red);
}
.tooltip.mod-top .tooltip-arrow {
  border-top: 5px solid var(--red);
}
body {
  --red: hsla(var(--interactive-accent-hsl), 0.9);
}
```
