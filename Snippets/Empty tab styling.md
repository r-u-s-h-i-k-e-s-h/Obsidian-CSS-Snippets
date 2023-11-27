↪[Collection](Collection.md)

# Empty tab styling

---

- author:: sai1494
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1052346864055369808

---

cover:: ![](https://i.imgur.com/MsmvCh8.gif)

```css
/*
author: sai1494
source: https://discord.com/channels/686053708261228577/702656734631821413/1052346864055369808
*/

.empty-state-container {
  max-height: unset;
  opacity: 1 !important;
}

.theme-dark .empty-state-container::before {
  content: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' shape-rendering='auto' viewBox='0 0 100 100' width='250' height='300' fill='none' stroke='gray' stroke-width='2' stroke-linecap='round' stroke-linejoin='bevel' class='logo-wireframe'%3E%3Cpath d='M 30.91 17.52 L 34.43 35.7 M 61.44 14.41 L 62.61 0 M 34.43 35.7 L 37.57 90.47 M 81 26.39 L 61.44 14.41 L 34.43 35.7 L 65.35 100 M 62.61 0 L 30.91 17.52 L 18 45.45 L 37.57 90.47 L 65.35 100 L 70.44 89.8 L 81 26.39 L 62.61 0 Z'%3E%3C/path%3E%3C/svg%3E");
  opacity: 30%;
}

.theme-light .empty-state-container::before {
  content: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' shape-rendering='auto' viewBox='0 0 100 100' width='250' height='300' fill='none' stroke='rgb(0, 0, 0)' stroke-width='2' stroke-linecap='round' stroke-linejoin='bevel' class='logo-wireframe'%3E%3Cpath d='M 30.91 17.52 L 34.43 35.7 M 61.44 14.41 L 62.61 0 M 34.43 35.7 L 37.57 90.47 M 81 26.39 L 61.44 14.41 L 34.43 35.7 L 65.35 100 M 62.61 0 L 30.91 17.52 L 18 45.45 L 37.57 90.47 L 65.35 100 L 70.44 89.8 L 81 26.39 L 62.61 0 Z'%3E%3C/path%3E%3C/svg%3E");
  opacity: 5%;
}

.empty-state-container:hover::before {
  content: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' shape-rendering='auto' viewBox='0 0 100 100' width='250' height='300' class='logo-full'%3E%3Cdefs%3E%3ClinearGradient id='a' x1='82.85' y1='30.41' x2='51.26' y2='105.9' gradientTransform='matrix(1, 0, 0, -1, -22.41, 110.97)' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%236c56cc'%3E%3C/stop%3E%3Cstop offset='1' stop-color='%239785e5'%3E%3C/stop%3E%3C/linearGradient%3E%3C/defs%3E%3Cpolygon points='62.61,0 30.91,17.52 18,45.45 37.57,90.47 65.35,100 70.44,89.8 81,26.39 62.61,0' fill='%2334208c'%3E%3C/polygon%3E%3Cpolygon points='81,26.39 61.44,14.41 34.43,35.7 65.35,100 70.44,89.8 81,26.39' fill='url(%23a)'%3E%3C/polygon%3E%3Cpolygon points='81,26.39 81,26.39 62.61,0 61.44,14.41 81,26.39' fill='%23af9ff4'%3E%3C/polygon%3E%3Cpolygon points='61.44,14.41 62.61,0 30.91,17.52 34.43,35.7 61.44,14.41' fill='%234a37a0'%3E%3C/polygon%3E%3Cpolygon points='34.43,35.7 37.57,90.47 65.35,100 34.43,35.7' fill='%234a37a0'%3E%3C/polygon%3E%3C/svg%3E");
  opacity: 100%;
  transition: opacity 1000ms cubic-bezier(0.25, 0.8, 0.25, 1);
}

.empty-state-title {
  display: none;
}
```
