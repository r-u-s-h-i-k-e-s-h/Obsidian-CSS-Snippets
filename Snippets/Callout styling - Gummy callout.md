↪[Collection](Collection.md)

# Callout styling - Gummy callout

---

- author:: kneecaps
- source:: https://discord.com/channels/686053708261228577/744933215063638183/1114979796250787890

---

cover:: ![](https://i.imgur.com/uOW5VRg.png)

```css
/*
author: kneecaps
source: https://discord.com/channels/686053708261228577/744933215063638183/1114979796250787890
*/

.callout[data-callout="abstract"],
.callout[data-callout="warning"],
.callout[data-callout="info"],
.callout[data-callout="example"],
.callout[data-callout="note"],
.callout[data-callout="tip"],
.callout[data-callout="success"],
.callout[data-callout="question"],
.callout[data-callout="failure"],
.callout[data-callout="danger"],
.callout[data-callout="bug"],
.callout[data-callout="quote"] {
  color: var(--color-callout-text);
}

.theme-dark {
  --color-callout-red: #502626;
  --color-callout-blue: #263850;
  --color-callout-green: #265029;
  --color-callout-yellow: #4c5026;
  --color-callout-orange: #504126;
  --color-callout-teal: #264e50;
  --color-callout-grey: #3b3b3b;
  --color-callout-purple: #392650;

  --color-callout-border-red: #715050;
  --color-callout-border-blue: #516073;
  --color-callout-border-green: #507153;
  --color-callout-border-yellow: #6e7150;
  --color-callout-border-orange: #716550;
  --color-callout-border-teal: #507171;
  --color-callout-border-grey: #616161;
  --color-callout-border-purple: #472650;
  --color-callout-text: var(--text-on-accent);
}

.theme-light {
  --color-callout-red: #ffe0e0;
  --color-callout-blue: #def1ff;
  --color-callout-green: #e0ffe3;
  --color-callout-yellow: #ffffe0;
  --color-callout-orange: #fff2e0;
  --color-callout-teal: #e0feff;
  --color-callout-grey: #ededed;
  --color-callout-purple: #ede0ff;

  --color-callout-border-red: #e5c7c7;
  --color-callout-border-blue: #c7d8e5;
  --color-callout-border-green: #cce5c7;
  --color-callout-border-yellow: #e3e5c7;
  --color-callout-border-orange: #e5dbc7;
  --color-callout-border-teal: #c7e5e5;
  --color-callout-border-grey: #dbdbdb;
  --color-callout-border-purple: #d8c7e5;
  --color-callout-text: var(--text-normal);
}

.callout[data-callout="info"],
.callout[data-callout="todo"] {
  border: 1px solid var(--color-callout-border-blue);
  background: var(--color-callout-blue);
}

.callout[data-callout="abstract"],
.callout[data-callout="summary"],
.callout[data-callout="tldr"] {
  border: 1px solid var(--color-callout-border-teal);
  background: var(--color-callout-teal);
}

.callout[data-callout="warning"],
.callout[data-callout="caution"],
.callout[data-callout="danger"] {
  border: 1px solid var(--color-callout-border-orange);
  background: var(--color-callout-orange);
}

.callout[data-callout="example"] {
  border: 1px solid var(--color-callout-border-purple);
  background: var(--color-callout-purple);
}

.callout[data-callout="note"] {
  border: 1px solid var(--color-callout-border-blue);
  background: var(--color-callout-blue);
}

.callout[data-callout="tip"],
.callout[data-callout="hint"],
.callout[data-callout="important"] {
  border: 1px solid var(--color-callout-border-teal);
  background: var(--color-callout-teal);
}

.callout[data-callout="question"],
.callout[data-callout="help"],
.callout[data-callout="faq"] {
  border: 1px solid var(--color-callout-border-yellow);
  background: var(--color-callout-yellow);
}

.callout[data-callout="danger"],
.callout[data-callout="error"] {
  border: 1px solid var(--color-callout-border-red);
  background: var(--color-callout-red);
}

.callout[data-callout="failure"],
.callout[data-callout="fail"],
.callout[data-callout="missing"] {
  border: 1px solid var(--color-callout-border-red);
  background: var(--color-callout-red);
}

.callout[data-callout="bug"] {
  border: 1px solid var(--color-callout-border-red);
  background: var(--color-callout-red);
}

.callout[data-callout="quote"],
.callout[data-callout="cite"] {
  border: 1px solid var(--color-callout-border-grey);
  background: var(--color-callout-grey);
}

.callout[data-callout="success"],
.callout[data-callout="check"],
.callout[data-callout="done"] {
  border: 1px solid var(--color-callout-border-green);
  background: var(--color-callout-green);
}

.callout {
  border-radius: 8px;
  transition: 700ms;
}

.callout:hover {
  transform: translateY(4px);
}

.callout-title-inner {
  color: var(--color-base-100);
}

.callout[data-callout="todo"] {
  border: 1px solid rgb(255, 204, 112);
  background: linear-gradient(
    43deg,
    rgb(65, 88, 208) 0%,
    rgb(200, 80, 192) 46%,
    rgb(255, 204, 112) 100%
  );
}

.callout[data-callout="tldr"] {
  border: 1px solid #07f49e;
  background: linear-gradient(43deg, #42047e 0%, #07f49e 100%);
}

.callout[data-callout="missing"] {
  border: 1px solid #ef745c;
  background: linear-gradient(43deg, #34073d 0%, #ef745c 100%);
}

.callout[data-callout="summary"] {
  border: 1px solid #ccb3d1;
  background: linear-gradient(43deg, #22052d 0%, #ccb3d1 100%);
}

.callout[data-callout="caution"] {
  border: 1px solid #557c93;
  background: linear-gradient(43deg, #08203e 0%, #557c93 100%);
}

.callout[data-callout="hint"] {
  border: 1px solid #a4c6b8;
  background: linear-gradient(43deg, #5e435d 0%, #a4c6b8 100%);
}

.callout[data-callout="help"],
.callout[data-callout="faq"] {
  border: 1px solid #5d5d3c;
  background: linear-gradient(43deg, #3f3f42 0%, #5d5d3c 100%);
}

.callout[data-callout="error"] {
  border: 1px solid #751006;
  background: linear-gradient(43deg, #1f0021 0%, #751006 100%);
}

.callout[data-callout="fail"] {
  border: 1px solid #f4985a;
  background: linear-gradient(43deg, #12243f 0%, #f4985a 100%);
}

.callout[data-callout="important"] {
  border: 1px solid #f9bc2c;
  background: linear-gradient(43deg, #f74c06 0%, #f9bc2c 100%);
}

.callout[data-callout="cite"] {
  border: 1px solid #858e96;
  background: linear-gradient(43deg, #60696b 0%, #858e96 100%);
}

.callout[data-callout="check"],
.callout[data-callout="done"] {
  border: 1px solid #99f2d1;
  background: linear-gradient(43deg, #1c3e35 0%, #99f2d1 100%);
}

.callout[data-callout="tldr"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(66, 4, 126, 0.4), 24px -24px 69px -3px
      rgba(7, 244, 158, 0.1);
}

.callout[data-callout="caution"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(52, 7, 61, 0.3), 24px -24px 69px -3px
      rgba(239, 116, 92, 0.3);
}

.callout[data-callout="todo"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(84, 86, 206, 0.3), 0px 1px 69px -3px
      rgba(201, 88, 187, 0.3), 24px -24px 69px -3px rgba(250, 191, 120, 0.3);
}

.callout[data-callout="summary"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(34, 5, 45, 0.3), 24px -24px 69px -3px
      rgba(239, 116, 92, 0.2);
}

.callout[data-callout="caution"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(8, 32, 62, 0.3), 24px -24px 69px -3px
      rgba(85, 124, 147, 0.3);
}

.callout[data-callout="hint"]:hover,
.callout[data-callout="important"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(94, 67, 93, 0.3), 24px -24px 69px -3px
      rgba(164, 198, 184, 0.3);
}

.callout[data-callout="check"]:hover,
.callout[data-callout="done"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(28, 62, 53, 0.3), 24px -24px 69px -3px
      rgba(153, 242, 209, 0.3);
}

.callout[data-callout="help"]:hover,
.callout[data-callout="faq"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(63, 63, 66, 0.3), 24px -24px 69px -3px
      rgba(93, 93, 60, 0.3);
}

.callout[data-callout="fail"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(18, 36, 63, 0.3), 24px -24px 69px -3px
      rgba(244, 152, 90, 0.3);
}

.callout[data-callout="error"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(31, 0, 33, 0.3), 24px -24px 69px -3px
      rgba(117, 16, 6, 0.3);
}

.callout[data-callout="important"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(249, 188, 44, 0.3), 24px -24px 69px -3px
      rgba(247, 76, 6, 0.3);
}

.callout[data-callout="cite"]:hover {
  box-shadow: -24px 24px 69px -3px rgba(96, 105, 107, 0.3), 24px -24px 69px -3px
      rgba(133, 142, 150, 0.3);
}

.callout[data-callout="tldr"]:hover,
.callout[data-callout="caution"]:hover,
.callout[data-callout="todo"]:hover,
.callout[data-callout="summary"]:hover,
.callout[data-callout="hint"]:hover,
.callout[data-callout="important"]:hover,
.callout[data-callout="check"]:hover,
.callout[data-callout="done"]:hover,
.callout[data-callout="help"]:hover,
.callout[data-callout="faq"]:hover,
.callout[data-callout="fail"]:hover,
.callout[data-callout="error"]:hover,
.callout[data-callout="important"]:hover,
.callout[data-callout="cite"]:hover {
  border: 1px solid white;
}

.callout[data-callout="tldr"],
.callout[data-callout="caution"],
.callout[data-callout="todo"],
.callout[data-callout="summary"],
.callout[data-callout="hint"],
.callout[data-callout="important"],
.callout[data-callout="check"],
.callout[data-callout="done"],
.callout[data-callout="help"],
.callout[data-callout="faq"],
.callout[data-callout="fail"],
.callout[data-callout="error"],
.callout[data-callout="important"],
.callout[data-callout="cite"] {
  color: white;
}

.callout[data-callout="tldr"] .callout-title-inner,
.callout[data-callout="caution"] .callout-title-inner,
.callout[data-callout="todo"] .callout-title-inner,
.callout[data-callout="summary"] .callout-title-inner,
.callout[data-callout="hint"] .callout-title-inner,
.callout[data-callout="important"] .callout-title-inner,
.callout[data-callout="check"] .callout-title-inner,
.callout[data-callout="done"] .callout-title-inner,
.callout[data-callout="help"] .callout-title-inner,
.callout[data-callout="faq"] .callout-title-inner,
.callout[data-callout="fail"] .callout-title-inner,
.callout[data-callout="error"] .callout-title-inner,
.callout[data-callout="important"] .callout-title-inner,
.callout[data-callout="cite"] .callout-title-inner {
  color: white;
}
```
