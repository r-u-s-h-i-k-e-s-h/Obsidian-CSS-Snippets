↪[Collection](Collection.md)

# Callout styling - Timeline callout

---

- author:: FireIsGood
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1156868388249935883

---

> _There might be some conflict if you are using_ **SlRvb's callout adjustment or ITS theme**

cover:: ![](https://i.imgur.com/UzllmA4.png)

```css
/*
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1156868388249935883
*/

/* Timeline Callout settings */
body {
  --timeline-title-color: var(--text-normal);
  --timeline-title-size: var(--h2-size);
  --timeline-title-width: 150px;

  --timeline-line-color: var(--color-base-35);
  --timeline-line-margin: 16px;
  --timeline-line-width: 4px;
  --timeline-line-style: solid;

  --timeline-dot-color: var(--color-base-70);
  --timeline-dot-size: 32px;
  --timeline-dot-radius: 100%;
  --timeline-dot-border-color: var(--background-primary);
  --timeline-dot-border-size: 6px;
  --timeline-dot-offset-x: -18px;
  --timeline-dot-offset-y: -2px;

  --timeline-card-margin: 16px;
  --timeline-card-background-color: var(--color-base-30);
  --timeline-card-padding-x: 10px;
  --timeline-card-padding-y: 16px;
}

/* Timeline styling */
[data-callout="timeline"] {
  order: 1;
  padding: 0;
  margin: 0;
  display: grid;
  mix-blend-mode: normal;
  background-color: unset;
  grid-template-columns: var(--timeline-title-width, 150px) auto;
  --dot-offset: calc(
    var(--timeline-dot-offset-y) + var(--timeline-card-padding-y)
  );

  .callout-title-inner {
    width: 100%;
    text-align: right;
    color: var(--timeline-title-color);
    font-size: var(--timeline-title-size);
    margin-top: var(--dot-offset);
  }
  .callout-icon {
    order: 2;
    margin-inline: var(--timeline-line-margin);
    border-left: var(--timeline-line-width) var(--timeline-line-style) var(--timeline-line-color);
    height: 100%;
    position: relative;

    &::after {
      content: "";
      box-sizing: border-box;
      background-color: var(--timeline-dot-color);
      position: absolute;
      border: var(--timeline-dot-border-size) solid var(
          --timeline-dot-border-color
        );
      border-radius: var(--timeline-dot-radius);
      width: var(--timeline-dot-size);
      height: var(--timeline-dot-size);
      top: var(--dot-offset);
      left: var(--timeline-dot-offset-x);
    }
  }
  .svg-icon {
    display: none;
  }

  .callout-content {
    order: 3;
    --p-spacing: 0.5rem;
    background-color: var(--timeline-card-background-color);
    border-radius: 1rem;
    margin-bottom: var(--timeline-card-margin);
    padding: var(--timeline-card-padding-x) var(--timeline-card-padding-y);

    & > h2:first-child {
      margin-top: 0;
    }
  }
}

/* Stacking multiple timelines */
div:not(:has(> [data-callout="timeline"])) + div > [data-callout="timeline"] {
  margin-top: var(--p-spacing);
}
div:has(> [data-callout="timeline"]) + div:not(> [data-callout="timeline"]) {
  margin-bottom: 1rem;
}

/* Timeline dot colors */
[data-callout-metadata="red"] {
  --timeline-dot-color: var(--color-red);
}
[data-callout-metadata="orange"] {
  --timeline-dot-color: var(--color-orange);
}
[data-callout-metadata="yellow"] {
  --timeline-dot-color: var(--color-yellow);
}
[data-callout-metadata="green"] {
  --timeline-dot-color: var(--color-green);
}
[data-callout-metadata="cyan"] {
  --timeline-dot-color: var(--color-cyan);
}
[data-callout-metadata="blue"] {
  --timeline-dot-color: var(--color-blue);
}
[data-callout-metadata="purple"] {
  --timeline-dot-color: var(--color-purple);
}
[data-callout-metadata="pink"] {
  --timeline-dot-color: var(--color-pink);
}
```

---

## How to use

```md
> [!timeline|red] Title
> Lorem, ipsum dolor sit amet consectetur, adipisicing elit.
```
