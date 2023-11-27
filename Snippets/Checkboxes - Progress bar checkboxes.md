↪[Collection](Collection.md)

# Checkboxes - Progress bar checkboxes

---

- author:: quinntyx, sailKite
- source:: https://discord.com/channels/686053708261228577/744933215063638183/1145481360757244065

---

cover:: ![](https://i.imgur.com/yJDlOAx.png)

```css
/*
author: quinntyx, sailKite
source: https://discord.com/channels/686053708261228577/744933215063638183/1145481360757244065
*/

body {
  --checkbox-progress-width: 55px;
  --checkbox-progress-radius: 10px;
  --checkbox-progress-border-width: 1px;
  --checkbox-progress-height: 12px;
  --checkbox-progress-background: initial;
  --checkbox-progress-unit-frac: 0.2;
  --checkbox-progress-animation-time: 600ms;
}

@keyframes checkbox-progress-transition {
  from {
    width: calc(
      var(--checkbox-progress-width) *
        (var(--progress-frac) - var(--checkbox-progress-unit-frac))
    );
  }
  to {
    width: calc(var(--checkbox-progress-width) * var(--progress-frac));
  }
}

input:is(.task-list-item-checkbox):is(
    [data-task="0"],
    [data-task="1"],
    [data-task="2"],
    [data-task="3"],
    [data-task="4"],
    [data-task="5"],
    :is(
        [data-task="0"],
        [data-task="1"],
        [data-task="2"],
        [data-task="3"],
        [data-task="4"],
        [data-task="5"]
      )
      > *
  ) {
  width: var(--checkbox-progress-width);
  border-radius: var(--checkbox-progress-radius);
  background: var(--checkbox-progress-background);
  border: var(--checkbox-progress-border-width) solid var(--interactive-accent);
  height: var(--checkbox-progress-height);
  transition: border var(--checkbox-progress-animation-time);

  &:hover {
    background: var(--checkbox-progress-background);
  }

  &::after {
    width: calc(var(--checkbox-progress-width) * var(--progress-frac));
    animation-name: checkbox-progress-transition;
    animation-duration: var(--checkbox-progress-animation-time);
    background: var(--interactive-accent) !important;
    margin-top: 1px;
    height: 100%;
    border-radius: var(--checkbox-progress-radius);
    -webkit-mask-image: none;
    mask-image: none; /* vsc is not happy since -webkit-mask-image is not cross-platform even though this does nothing */
  }
}
input.task-list-item-checkbox:is([data-task="0"], [data-task="0"] > *) {
  border: var(--checkbox-progress-border-width) solid var(
      --checkbox-border-color
    ) !important;
}
input.task-list-item-checkbox:is([data-task="0"], [data-task="0"] > *) {
  --progress-frac: 0;
}
input.task-list-item-checkbox:is([data-task="1"], [data-task="1"] > *) {
  --progress-frac: 0.2;
}
input.task-list-item-checkbox:is([data-task="2"], [data-task="2"] > *) {
  --progress-frac: 0.4;
}
input.task-list-item-checkbox:is([data-task="3"], [data-task="3"] > *) {
  --progress-frac: 0.6;
}
input.task-list-item-checkbox:is([data-task="4"], [data-task="4"] > *) {
  --progress-frac: 0.8;
}
input.task-list-item-checkbox:is([data-task="5"], [data-task="5"] > *) {
  --progress-frac: 1;
}
```

---

## How to use

```md
- [0] zero `0`
- [1] one `1`
- [2] two `2`
- [3] three `3`
- [4] four `4`
- [5] five `5`
```
