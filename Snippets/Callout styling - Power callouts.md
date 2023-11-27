↪[Collection](Collection.md)

# Callout styling - Power callouts

---

- author:: kneecaps
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1070521863761047593

---

> _You will need to turn it on using **style settings** plugin_

cover:: ![](https://i.imgur.com/bdbC8Pz.png)

```css
/*
author: kneecaps
source: https://discord.com/channels/686053708261228577/702656734631821413/1070521863761047593
*/

/* Style Settings*/
/* @settings
name: Power Callouts
id: power-callouts
settings:
  - 
    id: brutal
    title: Brutalist
    description: Sharp corners, thick border, heavy color demarking
    type: class-toggle
  - 
    id: soft
    title: Soft
    description: Rounded corners, duo-tone
    type: class-toggle
*/

.callout[data-callout="multi-column"]:hover {
  transform: translateY(0px);
}

.callout:hover {
  transform: translateY(4px);
}

.callout {
  transition: all 0.5s cubic-bezier(0.645, 0.045, 0.355, 1);
}

.callout[data-callout="shadow"] {
  --callout-title-color: var(--color-blue-rgb);
  --callout-color: var(--color-blue-rgb);
}

.callout[data-callout="shadow"] .callout-icon .svg-icon {
  background-color: var(--color-blue);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-layers-subtract' width='16' height='16' viewBox='0 0 24 24' stroke-width='1.5' stroke='%232c3e50' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'/%3E%3Crect x='8' y='4' width='12' height='12' rx='2' /%3E%3Cpath d='M16 16v2a2 2 0 0 1 -2 2h-8a2 2 0 0 1 -2 -2v-8a2 2 0 0 1 2 -2h2' /%3E%3C/svg%3E");
}

.callout[data-callout="sorcery"] {
  --callout-title-color: var(--color-red-rgb);
  --callout-color: var(--color-red-rgb);
}
.callout[data-callout="sorcery"] .callout-icon .svg-icon {
  background-color: var(--color-red);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-layers-union' width='16' height='16' viewBox='0 0 24 24' stroke-width='1.5' stroke='%232c3e50' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'/%3E%3Cpath d='M16 16v2a2 2 0 0 1 -2 2h-8a2 2 0 0 1 -2 -2v-8a2 2 0 0 1 2 -2h2v-2a2 2 0 0 1 2 -2h8a2 2 0 0 1 2 2v8a2 2 0 0 1 -2 2h-2' /%3E%3C/svg%3E");
}

.callout[data-callout="eidolon"] {
  --callout-title-color: var(--color-green-rgb);
  --callout-color: var(--color-green-rgb);
}
.callout[data-callout="eidolon"] .callout-icon .svg-icon {
  background-color: var(--color-green);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-layers-difference' width='16' height='16' viewBox='0 0 24 24' stroke-width='1.5' stroke='%232c3e50' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'/%3E%3Cpath d='M16 16v2a2 2 0 0 1 -2 2h-8a2 2 0 0 1 -2 -2v-8a2 2 0 0 1 2 -2h2v-2a2 2 0 0 1 2 -2h8a2 2 0 0 1 2 2v8a2 2 0 0 1 -2 2h-2' /%3E%3Cpolyline points='10 8 8 8 8 10' /%3E%3Cpolyline points='8 14 8 16 10 16' /%3E%3Cpolyline points='14 8 16 8 16 10' /%3E%3Cpolyline points='16 14 16 16 14 16' /%3E%3C/svg%3E");
}

.callout[data-callout="umbra"] {
  --callout-title-color: var(--color-purple-rgb);
  --callout-color: var(--color-purple-rgb);
}
.callout[data-callout="umbra"] .callout-icon .svg-icon {
  background-color: var(--color-purple);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-layers-intersect' width='16' height='16' viewBox='0 0 24 24' stroke-width='1.5' stroke='%232c3e50' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'/%3E%3Crect x='8' y='4' width='12' height='12' rx='2' /%3E%3Crect x='4' y='8' width='12' height='12' rx='2' /%3E%3C/svg%3E");
}

.brutal .callout {
  position: relative;
  overflow: visible;
  background: var(--background-primary);
  box-shadow: 8px 8px 0 -2.5px var(--background-primary), 8px 8px 0 0 rgb(var(--callout-color));
  border: 2.5px solid rgb(var(--callout-color));
  border-radius: 0px;
}

.brutal .callout:before {
  background: rgb(var(--callout-color));
  content: "";
  position: absolute;
  top: 8px;
  left: 8px;
  width: 100%;
  height: 100%;
  opacity: 0.2;
}

.soft .callout {
  position: relative;
  overflow: hidden;
}

.soft .callout:before {
  background: rgb(var(--callout-color));
  content: "";
  position: absolute;
  top: 64px;
  left: 0;
  width: 100%;
  height: 100%;
  opacity: 0.1;
  border-radius: 0px;
}
```
