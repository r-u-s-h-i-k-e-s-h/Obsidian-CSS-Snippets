---
author:
  - mrkcmn
source: https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets/pull/11
cover: "[[gif-empty tab - custom icon disappearing transition.gif]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Empty tab - custom icon disappearing transition

![](../attachments/gif-empty%20tab%20-%20custom%20icon%20disappearing%20transition.gif)

## Snippet

```css
/*
author: mrkcmn
source: https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets/pull/11
inspired by the emtpy tab - custom icon snippet by sai1494
*/

.empty-state-container {
  position: relative;
  top: -15%;
  left: 1%;
}

.empty-state-container:hover::before {
  content: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' shape-rendering='auto' viewBox='0 0 100 100' width='250' height='300' class='logo-full'%3E%3Cdefs%3E%3ClinearGradient id='a' x1='82.85' y1='30.41' x2='51.26' y2='105.9' gradientTransform='matrix(1, 0, 0, -1, -22.41, 110.97)' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%236c56cc'%3E%3C/stop%3E%3Cstop offset='1' stop-color='%239785e5'%3E%3C/stop%3E%3C/linearGradient%3E%3C/defs%3E%3Cpolygon points='62.61,0 30.91,17.52 18,45.45 37.57,90.47 65.35,100 70.44,89.8 81,26.39 62.61,0' fill='%2334208c'%3E%3C/polygon%3E%3Cpolygon points='81,26.39 61.44,14.41 34.43,35.7 65.35,100 70.44,89.8 81,26.39' fill='url(%23a)'%3E%3C/polygon%3E%3Cpolygon points='81,26.39 81,26.39 62.61,0 61.44,14.41 81,26.39' fill='%23af9ff4'%3E%3C/polygon%3E%3Cpolygon points='61.44,14.41 62.61,0 30.91,17.52 34.43,35.7 61.44,14.41' fill='%234a37a0'%3E%3C/polygon%3E%3Cpolygon points='34.43,35.7 37.57,90.47 65.35,100 34.43,35.7' fill='%234a37a0'%3E%3C/polygon%3E%3C/svg%3E");
  opacity: 100%;
  transition: opacity 1000ms cubic-bezier(0, 0.2, 0.8, 1);
  position: relative;
  z-index: 1;
}

.empty-state-container:not(:hover)::before {
  content: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' shape-rendering='auto' viewBox='0 0 100 100' width='250' height='300' class='logo-full'%3E%3Cdefs%3E%3ClinearGradient id='a' x1='82.85' y1='30.41' x2='51.26' y2='105.9' gradientTransform='matrix(1, 0, 0, -1, -22.41, 110.97)' gradientUnits='userSpaceOnUse'%3E%3Cstop offset='0' stop-color='%236c56cc'%3E%3C/stop%3E%3Cstop offset='1' stop-color='%239785e5'%3E%3C/stop%3E%3C/linearGradient%3E%3C/defs%3E%3Cpolygon points='62.61,0 30.91,17.52 18,45.45 37.57,90.47 65.35,100 70.44,89.8 81,26.39 62.61,0' fill='%2334208c'%3E%3C/polygon%3E%3Cpolygon points='81,26.39 61.44,14.41 34.43,35.7 65.35,100 70.44,89.8 81,26.39' fill='url(%23a)'%3E%3C/polygon%3E%3Cpolygon points='81,26.39 81,26.39 62.61,0 61.44,14.41 81,26.39' fill='%23af9ff4'%3E%3C/polygon%3E%3Cpolygon points='61.44,14.41 62.61,0 30.91,17.52 34.43,35.7 61.44,14.41' fill='%234a37a0'%3E%3C/polygon%3E%3Cpolygon points='34.43,35.7 37.57,90.47 65.35,100 34.43,35.7' fill='%234a37a0'%3E%3C/polygon%3E%3C/svg%3E");
  opacity: 0%;
  transition: opacity 1300ms cubic-bezier(0, 0.2, 0.8, 1);
  position: relative;
  z-index: 1;
}

.empty-state-title {
  position: absolute;
  top: -7.2%;
  left: 0.2%;
  z-index: 0;
  color: var(--background-primary);
}

.theme-dark .empty-state-title {
  content: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' shape-rendering='auto' viewBox='0 0 100 100' width='250' height='300' fill='none' stroke='gray' stroke-width='0.5' stroke-linecap='round' stroke-linejoin='bevel' class='logo-wireframe'%3E%3Cpath d='M 30.91 17.52 L 34.43 35.7 M 61.44 14.41 L 62.61 0 M 34.43 35.7 L 37.57 90.47 M 81 26.39 L 61.44 14.41 L 34.43 35.7 L 65.35 100 M 62.61 0 L 30.91 17.52 L 18 45.45 L 37.57 90.47 L 65.35 100 L 70.44 89.8 L 81 26.39 L 62.61 0 Z'%3E%3C/path%3E%3C/svg%3E");
  opacity: 40%;
}

.theme-light .empty-state-title {
  content: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' shape-rendering='auto' viewBox='0 0 100 100' width='250' height='300' fill='none' stroke='rgb(0, 0, 0)' stroke-width='2' stroke-linecap='round' stroke-linejoin='bevel' class='logo-wireframe'%3E%3Cpath d='M 30.91 17.52 L 34.43 35.7 M 61.44 14.41 L 62.61 0 M 34.43 35.7 L 37.57 90.47 M 81 26.39 L 61.44 14.41 L 34.43 35.7 L 65.35 100 M 62.61 0 L 30.91 17.52 L 18 45.45 L 37.57 90.47 L 65.35 100 L 70.44 89.8 L 81 26.39 L 62.61 0 Z'%3E%3C/path%3E%3C/svg%3E");
  opacity: 10%;
}
```
