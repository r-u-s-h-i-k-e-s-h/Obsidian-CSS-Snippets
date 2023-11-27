↪[Collection](Collection.md)

# Checkboxes - Origami theme

---

- author:: kneecaps
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1110960596129681520

---

cover:: ![](https://i.imgur.com/yp6CiNn.png)

```css
/*
author: kneecaps
source: https://discord.com/channels/686053708261228577/702656734631821413/1110960596129681520
*/

/* note checkboxes */
input[type="checkbox"] {
  height: var(--checkbox-size);
  width: var(--checkbox-size);

  background: var(--background-modifier-border);

  position: relative;

  padding: 0;
  margin: 0 6px 0 0;

  border: none;
  border-radius: var(--radius-s);

  transition: all 0.3s;

  -webkit-appearance: none;
  appearance: none;
  flex-shrink: 0;
}

/* .markdown-source-view.mod-cm6 .task-list-item-checkbox {
    top: 0px;
    vertical-align: text-top;
    margin-left: 2px;
} */

input[type="checkbox"]:hover {
  border: none;
  border-radius: var(--checkbox-radius);
  transition: box-shadow 0.15s ease-in-out;
  -webkit-appearance: none;
  appearance: none;
}

input[type="checkbox"]:checked {
  background: transparent;
  border: none;
  animation: pop 0.5s;
  animation-direction: alternate;
}

input[type="checkbox"]:checked::after {
  display: block;
  content: "";

  height: var(--checkbox-size);
  width: var(--checkbox-size);

  background: var(--text-accent);

  position: absolute;
  /* top: 2px;
	left: -2px; */

  -webkit-mask-position: 52% 52%;
  -webkit-mask-size: 100%;
  -webkit-mask-repeat: no-repeat;
  -webkit-mask-image: url('data:image/svg+xml,%3Csvg xmlns="http://www.w3.org/2000/svg" class="icon icon-tabler icon-tabler-check" width="24" height="24" viewBox="0 0 24 24" stroke-width="2" stroke="currentColor" fill="none" stroke-linecap="round" stroke-linejoin="round"%3E%3Cpath stroke="none" d="M0 0h24v24H0z" fill="none"%3E%3C/path%3E%3Cpath d="M5 12l5 5l10 -10"%3E%3C/path%3E%3C/svg%3E');
  transition: 700ms;
}

li[data-task="x"] input[type="checkbox"]:checked::after {
  left: 1px;
}

input[type="checkbox"]:checked:hover {
  background: var(--text-on-accent);
  border: none;
  transform: scale(1.2);
  transition: 300ms;
}

input[type="checkbox"]:checked:hover::after {
  background: var(--color-accent);
}

@keyframes pop {
  0% {
    transform: scale(1);
  }

  50% {
    transform: scale(0.9);
  }

  100% {
    transform: scale(1);
  }
}

/* original code from the amazing sanctum theme (that theme got me into themeing, i love it so much!) */
.markdown-source-view.mod-cm6 .HyperMD-task-line[data-task="x"],
.markdown-source-view.mod-cm6 .HyperMD-task-line[data-task="X"],
ul > li.task-list-item[data-task="x"],
ul > li.task-list-item[data-task="X"] {
  text-decoration: none;
  color: var(--text-faint);
}

li.is-checked:where(
    li[data-task="-"],
    li[data-task=">"],
    li[data-task="B"],
    li[data-task="X"],
    li[data-task="b"],
    li[data-task="!"],
    li[data-task="?"],
    li[data-task="i"],
    li[data-task="/"]
  )
  input[type="checkbox"],
.markdown-source-view
  input[type="checkbox"]:where(
    li[data-task="-"],
    li[data-task=">"],
    li[data-task="B"],
    li[data-task="X"],
    li[data-task="b"],
    li[data-task="!"],
    li[data-task="?"],
    li[data-task="i"],
    li[data-task="/"]
  ):checked {
  background: transparent;
  border-width: 0;
  pointer-events: none;
}

li.is-checked:where(
    li[data-task="-"],
    li[data-task=">"],
    li[data-task="B"],
    li[data-task="X"],
    li[data-task="b"],
    li[data-task="!"],
    li[data-task="?"],
    li[data-task="i"],
    li[data-task="/"]
  )
  input[type="checkbox"]:hover,
.markdown-source-view
  input[type="checkbox"]:where(
    li[data-task="-"],
    li[data-task=">"],
    li[data-task="B"],
    li[data-task="X"],
    li[data-task="b"],
    li[data-task="!"],
    li[data-task="?"],
    li[data-task="i"],
    li[data-task="/"]
  ):checked:hover {
  box-shadow: none;
  border-color: transparent;
  pointer-events: none;
}

li.is-checked:where(
    li[data-task="-"],
    li[data-task=">"],
    li[data-task="B"],
    li[data-task="X"],
    li[data-task="b"],
    li[data-task="!"],
    li[data-task="?"],
    li[data-task="i"],
    li[data-task="/"]
  )
  input[type="checkbox"]::after,
.markdown-source-view
  input[type="checkbox"]:where(
    li[data-task="-"],
    li[data-task=">"],
    li[data-task="B"],
    li[data-task="X"],
    li[data-task="b"],
    li[data-task="!"],
    li[data-task="?"],
    li[data-task="i"],
    li[data-task="/"]
  ):checked::after {
  left: 0;
  -webkit-mask-size: 110%;
  pointer-events: none;
}

/* .markdown-source-view.mod-cm6 input[type="checkbox"][data-task] {
	top: -3px;
} */

li[data-task="!"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="!"]::after {
  background: var(--color-red);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-urgent' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Cpath d='M8 16v-4a4 4 0 0 1 8 0v4'%3E%3C/path%3E%3Cpath d='M3 12h1m8 -9v1m8 8h1m-15.4 -6.4l.7 .7m12.1 -.7l-.7 .7'%3E%3C/path%3E%3Crect x='6' y='16' width='12' height='4' rx='1'%3E%3C/rect%3E%3C/svg%3E");
}

li[data-task="?"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="?"]::after {
  background: var(--color-blue);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-question-circle' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Cpath d='M12 16v.01'%3E%3C/path%3E%3Cpath d='M12 13a2.003 2.003 0 0 0 .914 -3.782a1.98 1.98 0 0 0 -2.414 .483'%3E%3C/path%3E%3Ccircle cx='12' cy='12' r='9'%3E%3C/circle%3E%3C/svg%3E");
}

/* progress */
li[data-task="/"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="/"]::after {
  background: var(--color-yellow);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-hourglass-high' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Cpath d='M6.5 7h11'%3E%3C/path%3E%3Cpath d='M6 20v-2a6 6 0 1 1 12 0v2a1 1 0 0 1 -1 1h-10a1 1 0 0 1 -1 -1z'%3E%3C/path%3E%3Cpath d='M6 4v2a6 6 0 1 0 12 0v-2a1 1 0 0 0 -1 -1h-10a1 1 0 0 0 -1 1z'%3E%3C/path%3E%3C/svg%3E");
}

/* cancel */
li[data-task="-"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="-"]::after {
  background: var(--color-red);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-circle-minus' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Ccircle cx='12' cy='12' r='9'%3E%3C/circle%3E%3Cline x1='9' y1='12' x2='15' y2='12'%3E%3C/line%3E%3C/svg%3E");
}

/* defer */
li[data-task=">"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task=">"]::after {
  background: var(--color-orange);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-arrow-back' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Cpath d='M9 11l-4 4l4 4m-4 -4h11a4 4 0 0 0 0 -8h-1'%3E%3C/path%3E%3C/svg%3E");
}

li[data-task="<"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="<"]::after {
  background: var(--color-purple);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' viewBox='0 0 32 32'%3E%3Cpath d='M26 4h-4V2h-2v2h-8V2h-2v2H6a2.002 2.002 0 0 0-2 2v20a2.002 2.002 0 0 0 2 2h20a2.002 2.002 0 0 0 2-2V6a2.002 2.002 0 0 0-2-2ZM6 6h4v2h2V6h8v2h2V6h4v4H6Zm0 6h5v6H6Zm13 14h-6v-6h6Zm0-8h-6v-6h6Zm2 8v-6h5l.001 6Z'/%3E%3Cpath fill='none' d='M0 0h32v32H0z' data-name='&lt;Transparent Rectangle&gt;'/%3E%3C/svg%3E");
}

/* failed */
li[data-task="X"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="X"]::after {
  background: var(--color-red);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-trash-x' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Cpath d='M4 7h16'%3E%3C/path%3E%3Cpath d='M5 7l1 12a2 2 0 0 0 2 2h8a2 2 0 0 0 2 -2l1 -12'%3E%3C/path%3E%3Cpath d='M9 7v-3a1 1 0 0 1 1 -1h4a1 1 0 0 1 1 1v3'%3E%3C/path%3E%3Cpath d='M10 12l4 4m0 -4l-4 4'%3E%3C/path%3E%3C/svg%3E");
}

/* idea */
li[data-task="i"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="i"]::after {
  background: var(--color-green);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-seeding' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Cpath d='M12 10a6 6 0 0 0 -6 -6h-3v2a6 6 0 0 0 6 6h3'%3E%3C/path%3E%3Cpath d='M12 14a6 6 0 0 1 6 -6h3v1a6 6 0 0 1 -6 6h-3'%3E%3C/path%3E%3Cline x1='12' y1='20' x2='12' y2='10'%3E%3C/line%3E%3C/svg%3E");
}

/* brainstorm */
li[data-task="b"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="b"]::after {
  background: var(--color-purple);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-brain' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Cpath d='M15.5 13a3.5 3.5 0 0 0 -3.5 3.5v1a3.5 3.5 0 0 0 7 0v-1.8'%3E%3C/path%3E%3Cpath d='M8.5 13a3.5 3.5 0 0 1 3.5 3.5v1a3.5 3.5 0 0 1 -7 0v-1.8'%3E%3C/path%3E%3Cpath d='M17.5 16a3.5 3.5 0 0 0 0 -7h-.5'%3E%3C/path%3E%3Cpath d='M19 9.3v-2.8a3.5 3.5 0 0 0 -7 0'%3E%3C/path%3E%3Cpath d='M6.5 16a3.5 3.5 0 0 1 0 -7h.5'%3E%3C/path%3E%3Cpath d='M5 9.3v-2.8a3.5 3.5 0 0 1 7 0v10'%3E%3C/path%3E%3C/svg%3E");
}

/* bookmark */
li[data-task="B"] input[type="checkbox"]:checked::after,
input[type="checkbox"][data-task="B"]::after {
  background: var(--color-red);
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' class='icon icon-tabler icon-tabler-bookmark' width='24' height='24' viewBox='0 0 24 24' stroke-width='2' stroke='currentColor' fill='none' stroke-linecap='round' stroke-linejoin='round'%3E%3Cpath stroke='none' d='M0 0h24v24H0z' fill='none'%3E%3C/path%3E%3Cpath d='M9 4h6a2 2 0 0 1 2 2v14l-5 -3l-5 3v-14a2 2 0 0 1 2 -2'%3E%3C/path%3E%3C/svg%3E");
}
```
