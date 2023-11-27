↪[Collection](Collection.md)

# Loading screen tweak

---

- author:: FireIsGood
- source:: https://codepen.io/fireisgood/pen/eYQmyPJ

---

cover:: ![](https://i.imgur.com/na2WAxm.gif)

```css
/*
author: FireIsGood
source: https://codepen.io/fireisgood/pen/eYQmyPJ
*/

*,
*::after,
*::before {
  box-sizing: border-box;
}
@import url("https://fonts.googleapis.com/css2?family=Noto+Sans&display=swap");

.progress-bar {
  position: absolute;
  height: 100vh;
  width: 100vw;
  top: 0;
  left: 0;
  background-color: var(--background-primary);
  z-index: 10000;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
.progress-bar-message {
  margin-bottom: var(--size-4-8);
  opacity: 1;
  color: var(--text-muted);
}
.progress-bar-indicator {
  position: relative;
  height: 8px;
  margin: 0 10vw;
  width: 90vw;
  overflow-x: hidden;
  border-radius: 3px;
}
.progress-bar-line {
  position: absolute;
  opacity: 0.4;
  background-color: var(--interactive-accent);
  width: 150%;
  height: 8px;
}
.progress-bar-subline {
  position: absolute;
  background-color: var(--interactive-accent);
  height: 8px;
}
.progress-bar-subline.mod-increase {
  animation: increase 2s infinite;
}
.progress-bar-subline.mod-decrease {
  animation: decrease 2s 0.5s infinite;
}
.progress-bar .progress-bar-subline {
  transition: width 150ms ease-in-out;
}
@keyframes increase {
  from {
    left: -5%;
    width: 5%;
  }
  to {
    left: 130%;
    width: 100%;
  }
}
@keyframes decrease {
  from {
    left: -80%;
    width: 80%;
  }
  to {
    left: 110%;
    width: 10%;
  }
}

/**** My code ****/

/* Text trees */

.progress-bar-message::before {
  content: "🌺 ";
}
.progress-bar-message::after {
  content: " 🌺";
}

/* Progress bars */

body {
  --bar-height: 64px;
}

.progress-bar-indicator {
  height: var(--bar-height);
  overflow-y: hidden;
}
.progress-bar-indicator {
  border-radius: var(--bar-height);
}
.progress-bar-line,
.progress-bar-subline {
  overflow: hidden;
  border-radius: var(--bar-height);
  height: 100%;
  display: grid;
  place-items: center;
}

:root .progress-bar-subline {
  animation-duration: 8s;
  animation-timing-function: ease-out;
}
:root .mod-decrease {
  animation-name: increase-special;
}
:root .mod-decrease {
  animation-name: decrease-special;
  animation-delay: 2s;
}

.progress-bar-subline::before {
  content: "";
  height: 100%;
  aspect-ratio: 1/1;
  background-image: url("https://d1w8c6s6gmwlek.cloudfront.net/retrogametees.com/overlays/179/236/17923636.png");
  background-size: cover;
  background-position: top -25% center;
}
/* .mod-decrease::before {
  right: 0;
  text-align: left;
} */

@keyframes increase-special {
  from {
    left: 0%;
    width: 0%;
  }
  to {
    left: 120%;
    width: 100%;
  }
}

@keyframes decrease-special {
  from {
    left: -100%;
    width: 100%;
  }
  to {
    left: 120%;
    width: 0%;
  }
}
```
