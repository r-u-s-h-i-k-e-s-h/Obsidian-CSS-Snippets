---
author: rushi
reference: https://discord.com/channels/686053708261228577/702656734631821413/1096863934100807701
cover: "[[img-callout styling - author callout.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - author callout

![](../attachments/img-callout%20styling%20-%20author%20callout.webp)

## Snippet

```css
.callout[data-callout="author"] {
  display: flex;
  flex-direction: column;
  --callout-icon: user;
  --callout-color: var(--background-secondary-alt);
  box-shadow: var(--shadow-s);
  border-left: 4px solid var(--interactive-accent);
  border-radius: var(--radius-s);
  padding: var(--size-4-3) var(--size-4-4);
}

.callout[data-callout="author"] .callout-content {
  order: 1;
}

.callout[data-callout="author"]>.callout-title {
  order: 2;
  display: flex;
  justify-content: flex-end;
  font-style: italic;
  font-size: var(--font-small);
  color: var(--text-muted);
  padding: 0;
}
```

## How to use

```md
> [!author] Cicero (attributed)
> Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam. Eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. Nemo enim ipsam voluptatem quia voluptas sit aspernatur aut odit aut fugit.
```