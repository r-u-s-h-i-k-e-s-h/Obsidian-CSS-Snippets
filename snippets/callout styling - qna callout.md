---
author: jetfiremaster
source: https://discord.com/channels/686053708261228577/702656734631821413/1430284483373961247
cover: "[[img-callout styling - qna callout.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - qna callout

![](../attachments/img-callout%20styling%20-%20qna%20callout.webp)

## Snippet

```css
/*
author: jetfiremaster
source: https://discord.com/channels/686053708261228577/702656734631821413/1430284483373961247
*/

/* QNA Callout */
body {
  --callout-qna-q-symbol-size: 3em;
  --callout-qna-a-symbol-size: 3em;
}

.theme-light {
  --callout-qna-bkgd-color: 180, 180, 190;
  --callout-qna-q-symbol-color: #f9911a;
  --callout-qna-a-symbol-color: #38c294;
  --callout-qna-title-color: #2f2d2d;
}

.theme-dark {
  --callout-qna-bkgd-color: 74, 74, 84;
  --callout-qna-q-symbol-color: #bf834a;
  --callout-qna-a-symbol-color: #7b8f76;
  --callout-qna-title-color: #dcdada;
}

.callout[data-callout="qna"] {
  --callout-color: var(--callout-qna-bkgd-color);
  --callout-title-color: var(--callout-qna-title-color);
  padding-top: calc(var(--callout-qna-q-symbol-size)*0.5);

  .callout-title::before {
    content: "Q";
    font-size: var(--callout-qna-q-symbol-size);
    font-family: "Bahnschrift", sans-serif;
    color: var(--callout-qna-q-symbol-color);
    position: absolute;
  }

  .callout-title {
    align-items: center;
  }

  .callout-title>* {
    margin-left: var(--callout-qna-q-symbol-size);
  }


  .callout-content::before {
    position: absolute;
    content: "A";
    font-size: var(--callout-qna-a-symbol-size);
    font-family: "Bahnschrift", sans-serif;
    color: var(--callout-qna-a-symbol-color);

  }

  .callout-content {
    padding-top: 8px;
  }

  .callout-content>* {
    margin-left: var(--callout-qna-a-symbol-size);
    margin-top: calc(var(--callout-qna-a-symbol-size)*0.33);
  }

  .callout-icon {
    display: none;
  }
}
```

## How to use

```md
> [!qna] Explain Newton's law of gravity
> Newton's law of gravity (also called Newton’s law of universal gravitation) describes how any two objects in the universe attract each other. It is one of the foundational ideas in physics.
>
> ## The Law (in words)
>
> Every mass attracts every other mass with a force that:
>
> 1. Increases with the mass of the objects
> 2. Decreases rapidly with distance between them (specifically, with the square of the distance)
>
>    ## Mathematical formula
>
>    $$F = G \frac{m_1 m_2}{r^2}$$
```
