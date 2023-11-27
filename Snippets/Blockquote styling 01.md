↪[Collection](Collection.md)

# Blockquote styling 01

---

- author:: kneecaps
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1042896580539330560

---

> _Only works in reading mode._

cover:: ![](https://i.imgur.com/B3fyyED.png)

```css
/*
author: kneecaps
source: https://discord.com/channels/686053708261228577/702656734631821413/1042896580539330560
*/

.theme-light {
  --cbs: 0px 2px 4px rgba(0, 0, 0, 0.01), 0px 4px 8px rgba(0, 0, 0, 0.01),
    0px 4px 8px rgba(0, 0, 0, 0.01), 0px 0px 12px rgba(0, 0, 0, 0.01),
    0px 2px 16px rgba(0, 0, 0, 0.01), 0px 4px 20px rgba(0, 0, 0, 0.01);
  --background-primary-alt-1: var(--background-primary);
}

.theme-dark {
  --cbs: 0px 2px 4px rgba(0, 0, 0, 0.05), 0px 4px 8px rgba(0, 0, 0, 0.03),
    0px 4px 8px rgba(0, 0, 0, 0.05), 0px 0px 12px rgba(0, 0, 0, 0.03),
    0px 2px 16px rgba(0, 0, 0, 0.03), 0px 4px 20px rgba(0, 0, 0, 0.02);
  --background-primary-alt-1: var(--background-primary-alt);
}

.markdown-preview-view blockquote {
  padding: 8px 12px 8px 32px;
  border: 2px dashed var(--background-primary-alt-1); /* put 'border: 0px;' if you dont want the dashed border! */
  color: var(--text-muted); /* this is the text color */
  position: relative;
  border-radius: 12px; /* this controls the quotes 'roundness' */
  box-shadow: var(--cbs);
  background: var(
    --background-primary-alt-1
  ); /* var(--background-primary-alt) gives better contrast in darkmode, var(--background-primary) is more minimal; */
}

.markdown-preview-view blockquote:before {
  content: "";
  position: absolute;
  left: 15px;
  top: 15px;
  width: 3px;
  height: calc(100% - 30px);
  background: var(
    --color-accent
  ); /* change this color to change the vertical bar in preview mode! */
  border-radius: var(--button-radius);
}

cite {
  color: var(--text-accent);
  text-align: end;
  display: block;
  padding-right: 1em;
}
```

---

## How to use

```md
> Lorem ipsum dolor sit amet, consectetur, adipisicing elit. Iure minus voluptates illum aspernatur officia vel officiis, et quis qui. Enim omnis officia sunt consectetur obcaecati repudiandae! Numquam, voluptas at, ab officiis recusandae, dolorum inventore quod iste cumque explicabo dicta quidem accusantium velit odit deleniti, ipsum commodi?
> <cite>Name of the author</cite>
```
