↪[Collection](Collection.md)

# Callout styling - Label callout

---

- author:: sailKite, Lunairee
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1073456247849881610

---

cover:: ![](https://i.imgur.com/vVuVZYy.png)

```css
/* original by Lunairee#2396 on Obsidian Discord */
.callout[data-callout-metadata*="label"] {
  --block-spacing: 1rem;
  --speaker-block-width: 20%;
  margin: 0px;
  padding: 0px;
  display: grid;
  grid-template-columns: var(--speaker-block-width) calc(100% - var(--speaker-block-width));
  background-color: var(--background-primary);
  border: none;
}

.callout[data-callout-metadata*="label"] .callout-title {
  display: inline-block;
  height: calc(100% - var(--block-spacing));
  text-align: right;
  border-right: 3px solid;
  padding-right: var(--block-spacing);
  flex: 1 0 auto;
}

.callout[data-callout-metadata*="label"] > * {
  margin-top: var(--block-spacing);
}

.callout[data-callout-metadata*="label"] > .callout-title > .callout-icon {
  display: none;
}

.callout[data-callout-metadata*="label"] > .callout-content {
  padding: 0px var(--block-spacing);
}
.callout[data-callout-metadata*="label"] > .callout-content > p:first-child {
  margin-top: 0px;
}
.callout[data-callout-metadata*="label"] > .callout-content > p:last-child {
  margin-bottom: 0px;
}
```

---

## How to use

```md
> [!bug|label] Lorem, ipsum dolor sit amet
> Lorem, ipsum dolor sit amet consectetur, adipisicing elit. Lorem, ipsum dolor sit amet consectetur, adipisicing elit.
```
