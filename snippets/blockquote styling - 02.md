---
author: ApolloGoneRogue
source: https://forum.obsidian.md/t/how-to-achieve-css-code-snippets/8474/244?u
cover: "[[img-blockquote styling - 02.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Blockquote styling - 02

> Only works in reading mode

![](../attachments/img-blockquote%20styling%20-%2002.webp)

## Snippet

```css
/*
author: ApolloGoneRogue
source: https://forum.obsidian.md/t/how-to-achieve-css-code-snippets/8474/244?u
*/

/* This snippet provides a style to blockquotes and to the <cite> element. */

/* for preview */
.markdown-preview-view blockquote {
  border-color: #1abf7f !important;
  border-left-width: 2px !important;
  background-image: linear-gradient(to right,
      rgba(26, 191, 127, 0.1),
      rgba(26, 191, 127, 0));
  font-size: 1em;
  line-height: 1.5em;
  margin: auto;
  margin-bottom: 10px;
  padding-top: 10px;
  padding-bottom: 10px;
  padding-right: 15px;
  width: 80%;
}

.markdown-preview-view blockquote {
  position: relative;
}

.markdown-preview-view blockquote:after {
  content: "\275D";
  position: absolute;
  top: 0.4em;
  left: -1em;
  font-size: 2.5em;
  color: #1abf7f;
}

cite {
  color: #1abf7f;
  text-align: end;
  display: block;
}
```

## How to use

```md
> Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam. Eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit.
> <cite>Cicero (attributed)</cite>
```