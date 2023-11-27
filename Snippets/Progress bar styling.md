↪[Collection](Collection.md)

# Progress bar styling

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1160777103948656681

---

cover:: ![](https://i.imgur.com/KNfB1GQ.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1160777103948656681
*/

/* basic star rating system using progress elements */
:is(
    .markdown-preview-view,
    .markdown-rendered,
    .markdown-source-view.is-live-preview
  )
  progress.star {
  --total-number-of-stars: 10;
  height: 20px;
  vertical-align: middle;
}
:is(
    .markdown-preview-view,
    .markdown-rendered,
    .markdown-source-view.is-live-preview
  )
  progress[value].star::-webkit-progress-bar {
  container: starprog / inline-size;
  border: none;
  box-shadow: none;
  /* background: transparent; */
}
:is(
    .markdown-preview-view,
    .markdown-rendered,
    .markdown-source-view.is-live-preview
  )
  progress[value].star::-webkit-progress-value {
  background-color: unset;
  background-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' width='24' height='24' viewBox='0 0 24 24' fill='none' stroke='dodgerblue' stroke-width='2' stroke-linecap='round' stroke-linejoin='round' class='lucide lucide-star'%3E%3Cpolygon points='12 2 15.09 8.26 22 9.27 17 14.14 18.18 21.02 12 17.77 5.82 21.02 7 14.14 2 9.27 8.91 8.26 12 2'/%3E%3C/svg%3E");
  background-size: calc(100cqw / var(--total-number-of-stars)) 100%;
}
```

---

## How to use

```md
<progress class="star" id="file" max="100" value="25">70%</progress>
<progress class="star" id="file" max="100" value="44">70%</progress>
<progress class="star" id="file" max="100" value="66">70%</progress>
<progress class="star" id="file" max="100" value="87">70%</progress>
<progress class="star" id="file" max="100" value="97">70%</progress>
```
