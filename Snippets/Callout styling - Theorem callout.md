↪[Collection](Collection.md)

# Callout styling - Theorem callout

---

- author:: sailKite, elevict
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1164269429543149598

---

cover:: ![](https://i.imgur.com/8QnNSCF.png)

```css
/*
author: sailKite, elevict
source: https://discord.com/channels/686053708261228577/702656734631821413/1164269429543149598
*/

.callout[data-callout="theorem"] {
  --callout-color: var(--text-normal);
  font-family: Times;
  background-color: rgb(0, 0, 0, 0);
  border: solid;
  border-radius: 6px;
}
.callout[data-callout="theorem"] .callout-icon {
  display: none;
}
.callout[data-callout="theorem"] .callout-title-inner {
  font-weight: revert;
}
.callout[data-callout="theorem"] .callout-content {
  font-style: italic;
}
```

---

## How to use

```md
> [!theorem] **Theorem 1.4.49** (Dominated convergence theorem).
> Let $(X,B,\mu)$ be a measure space, and let $f_1, f_2, \dots: X \rightarrow C$ be a sequence of measurable functions that converge pointwise $\mu$-almost everywhere to a measurable limit $f:X \rightarrow C$. Suppose that there is an unsigned absolutely integrable function $G:X \rightarrow [0,+\infty]$ such that $|f_n|$ are pointwise $\mu$-almost everywhere bounded by $G$ for each $n$. Then we have
> $$\lim_{n \rightarrow \infty}\int_{X}f_nd\mu = \int_{X}f~d\mu$$
```
