---
author: Adonis
source: https://discord.com/channels/686053708261228577/702656734631821413/1040111314963546142
cover: "[[img-callout styling - compact quote callout.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - compact quote callout

![](../attachments/img-callout%20styling%20-%20compact%20quote%20callout.webp)

## Snippet

```css
/*
author: Adonis
source: https://discord.com/channels/686053708261228577/702656734631821413/1040111314963546142
*/

.callout[data-callout="quote"] {
  --callout-padding: var(--size-4-3);
  --icon-size: 70px;
  max-width: 250px;
}

.callout[data-callout="quote"] .callout-title .callout-icon {
  margin: 0 auto;
}

.callout[data-callout="quote"] .callout-title .callout-title-inner {
  display: none;
}

.callout[data-callout="quote"] .callout-content {
  padding-top: 20px;
}

.callout[data-callout="quote"] .callout-content p {
  font-style: italic;
  text-align: center;
}

.callout[data-callout="quote"] .callout-content p:first-child {
  margin-top: 0;
}

.callout[data-callout="quote"] .callout-content p:last-child {
  font-style: normal;
  color: rgb(var(--ctp-yellow, 153, 122, 0));
  text-align: right;
  margin-bottom: 0;
}
```

## How to use

```md
> [!quote] Title
> Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam.
>
> \- ullamco laboris
```