↪[Collection](Collection.md)

# Heading indicators 02

---

- author:: Daniel, sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1155544494897365084

---

cover:: ![](https://i.imgur.com/4qQrLIN.png)

```css
/*
author: Daniel, sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1155544494897365084
*/

/*
    cssclass: 'numbered-headers'
    functionality: Adds numbers to headers in all views/modes, as well as the dynamic TOC plugin.
*/

/* inside Dynamic ToC */
.numbered-headers .dynamic-toc ol {
  list-style-type: none;
}
.numbered-headers .dynamic-toc ol {
  counter-reset: decimal;
}
.numbered-headers .dynamic-toc ol > li {
  display: block;
}
.numbered-headers .dynamic-toc ol > li::before {
  content: counters(decimal, ".") " ";
  counter-increment: decimal;
  color: var(--text-a) /* put your text var here or hardcode the color */;
}

/* headers */
/* h1 */
.numbered-headers div:has(> h1) {
  counter-increment: h1counter;
  counter-reset: h2counter;
}
.numbered-headers div:has(> h1) > h1::before {
  content: counter(h1counter) ". ";
  color: var(--text-accent);
}
/* h2 */
.numbered-headers h2 {
  counter-increment: h2counter;
  counter-reset: h3counter;
}
.numbered-headers h2::before {
  content: counter(h1counter) "." counter(h2counter) ". ";
  color: var(--text-accent);
}
/* h3 */
.numbered-headers div:has(> h3) {
  counter-increment: h3counter;
  counter-reset: h4counter;
}
.numbered-headers div:has(> h3) > h3::before {
  content: counter(h1counter) "." counter(h2counter) "." counter(h3counter) ". ";
  color: var(--text-accent);
}
/* h4 */
.numbered-headers div:has(> h4) {
  counter-increment: h4counter;
  counter-reset: h5counter;
}
.numbered-headers div:has(> h4) > h4::before {
  content: counter(h1counter) "." counter(h2counter) "." counter(h3counter) "." counter(
      h4counter
    )
    ". ";
  color: var(--text-accent);
}
/* h5 */
.numbered-headers div:has(> h5) {
  counter-increment: h5counter;
  counter-reset: h6counter;
}
.numbered-headers div:has(> h5) > h5::before {
  content: counter(h1counter) "." counter(h2counter) "." counter(h3counter) "." counter(
      h4counter
    )
    "." counter(h5counter) ". ";
  color: var(--text-accent);
}
/* h6 */
.numbered-headers div:has(> h6) {
  counter-increment: h6counter;
}
.numbered-headers div:has(> h6) > h6::before {
  content: counter(h1counter) "." counter(h2counter) "." counter(h3counter) "." counter(
      h4counter
    )
    "." counter(h5counter) "." counter(h6counter) ". ";
  color: var(--text-accent);
}

/* live preview */
.numbered-headers .HyperMD-header-1 {
  counter-increment: h1counter;
  counter-reset: h2counter;
}
.numbered-headers .HyperMD-header-1::before {
  content: counter(h1counter) ". ";
  color: var(--text-accent);
}
/* h2 */
.numbered-headers .HyperMD-header-2 {
  counter-increment: h2counter;
  counter-reset: h3counter;
}
.numbered-headers .HyperMD-header-2::before {
  content: counter(h1counter) "." counter(h2counter) ". ";
  color: var(--text-accent);
}
/* h3 */
.numbered-headers .HyperMD-header-3 {
  counter-increment: h3counter;
  counter-reset: h4counter;
}
.numbered-headers .HyperMD-header-3:before {
  content: counter(h1counter) "." counter(h2counter) "." counter(h3counter) ". ";
  color: var(--text-accent);
}
/* h4 */
.numbered-headers .HyperMD-header-4 {
  counter-increment: h4counter;
  counter-reset: h5counter;
}
.numbered-headers .HyperMD-header-4::before {
  content: counter(h1counter) "." counter(h2counter) "." counter(h3counter) "." counter(
      h4counter
    )
    ". ";
  color: var(--text-accent);
}
/* h5 */
.numbered-headers .HyperMD-header-5 {
  counter-increment: h5counter;
  counter-reset: h6counter;
}
.numbered-headers .HyperMD-header-5:before {
  content: counter(h1counter) "." counter(h2counter) "." counter(h3counter) "." counter(
      h4counter
    )
    "." counter(h5counter) ". ";
  color: var(--text-accent);
}
/* h6 */
.numbered-headers .HyperMD-header-6 {
  counter-increment: h6counter;
}
.numbered-headers .HyperMD-header-6::before {
  content: counter(h1counter) "." counter(h2counter) "." counter(h3counter) "." counter(
      h4counter
    )
    "." counter(h5counter) "." counter(h6counter) ". ";
  color: var(--text-accent);
}
```
