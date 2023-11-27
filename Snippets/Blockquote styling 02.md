↪[Collection](Collection.md)

# Blockquote styling 02

---

- author:: ApolloGoneRogue
- source:: https://forum.obsidian.md/t/how-to-achieve-css-code-snippets/8474/244?u

---

cover:: ![](https://i.imgur.com/KuFyzsu.png)

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
  background-image: linear-gradient(
    to right,
    rgba(26, 191, 127, 0.1),
    rgba(26, 191, 127, 0)
  );
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

---

## How to use

```md
> Lorem ipsum dolor sit amet, consectetur, adipisicing elit. Iure minus voluptates illum aspernatur officia vel officiis, et quis qui. Enim omnis officia sunt consectetur obcaecati repudiandae! Numquam, voluptas at, ab officiis recusandae, dolorum inventore quod iste cumque explicabo dicta quidem accusantium velit odit deleniti, ipsum commodi?
> <cite>Name of the author</cite>
```
