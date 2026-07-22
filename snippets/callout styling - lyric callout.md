---
author: rushi
source:
cover: "[[img-callout styling - lyric callout.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - lyric callout

![](../attachments/img-callout%20styling%20-%20lyric%20callout.webp)

## Snippet

```css
.callout[data-callout="lyric"] {
  --callout-color: transparent;
  border: none;
  background-color: var(--background-primary);
  box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.08);
  border-radius: 8px;
  margin: 1.5em 0;
}

.callout[data-callout="lyric"] .callout-title {
  display: none;
}

.callout[data-callout="lyric"] .callout-content {
  font-size: 0.9em;
  text-align: center;
  padding: 1.5rem 2rem;
  line-height: 1.6;
  font-style: italic;
  color: var(--text-muted);
}

.callout[data-callout="lyric"] .callout-content::after {
  content: "--- ♪ ♪ ♪ ---";
  display: block;
  margin-top: 1.2rem;
  color: var(--text-accent);
  font-style: normal;
  letter-spacing: 2px;
}
```

## How to use

```css
> [!lyric] title will not appear
> content...
```