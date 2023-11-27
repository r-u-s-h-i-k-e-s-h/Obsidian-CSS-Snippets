↪[Collection](Collection.md)

# Callout styling - Tabbed callout

---

- author:: FireIsGood
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1092995965583114341

---

cover:: ![](https://i.imgur.com/ai6x8Ha.gif)

```css
/*
author: FireIsGood
source: https://discord.com/channels/686053708261228577/702656734631821413/1092995965583114341
*/

[data-callout="tabbed"] {
  outline: 1px solid var(--color-base-30);
  border-radius: 0.5rem;
}
[data-callout="tabbed"] > .callout-content {
  padding: 0.25rem;

  display: grid;
  grid-template-columns: repeat(auto-fill, minmax(5rem, max-content));
  gap: 0 1rem;
}
[data-callout="tabbed"] > .callout-title {
  display: none;
}
[data-callout="tabbed"] > .callout-content p {
  margin: 0;
}
[data-callout="tabbed"] > .callout-content label > input {
  display: none;
}
[data-callout="tabbed"] > .callout-content label {
  width: 100%;
  display: inline-block;
  padding: 0.15rem 0.75ch;
  border-radius: 1rem;

  color: #ccc;
  background-color: #2e7d32;

  text-align: center;
  font-weight: bold;
  font-size: 1.15rem;
  cursor: pointer;
}
[data-callout="tabbed"] > .callout-content label:has(input:checked) {
  color: white;
  background-color: #8bc34a;
}
[data-callout="tabbed"]
  > .callout-content
  p:not(:has(label input:checked))
  + blockquote {
  display: none;
}
[data-callout="tabbed"] > .callout-content > blockquote {
  order: 999;
  grid-column: 1 / -1;

  background-color: transparent;
  padding-left: 0;
  border: 0;
}
```

---

## How to use

```md
> [!tabbed]
>
> <label>First<input type="radio" name="test" />l</label>
>
> > Lorem, ipsum dolor sit amet consectetur, adipisicing elit. (First)
> > [[Obsidian CSS|Internal Link]] > > **bold** _italic_
>
> <label>Second<input type="radio" name="test" /></label>
>
> > Lorem, ipsum dolor sit amet consectetur, adipisicing elit. (Second)
> > [External Link](https://google.com) > > $\LaTeX$
>
> <label>Third<input type="radio" name="test" />l</label>
>
> > Lorem, ipsum dolor sit amet consectetur, adipisicing elit. (Third)
> >
> > - bullet item
> > - [ ] checkbox
> > - [x] #tag
```
