↪[Collection](Collection.md)

# Canvas styling - Gradient canvas cards

---

- author:: kneecaps
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1095868229634773143

---

cover:: ![](https://i.imgur.com/EtCIye8.png)

```css
/* 
author: kneecaps
source: https://discord.com/channels/686053708261228577/702656734631821413/1095868229634773143
*/

.canvas-node.is-themed.mod-canvas-color-1
  .canvas-node-content
  .markdown-preview-view
  .inline-title {
  color: rgb(var(--color-red-rgb));
}

.canvas-node.is-themed.mod-canvas-color-2
  .canvas-node-content
  .markdown-preview-view
  .inline-title {
  color: rgb(var(--color-orange-rgb));
}

.canvas-node.is-themed.mod-canvas-color-3
  .canvas-node-content
  .markdown-preview-view
  .inline-title {
  color: rgb(var(--color-yellow-rgb));
}

.canvas-node.is-themed.mod-canvas-color-4
  .canvas-node-content
  .markdown-preview-view
  .inline-title {
  color: rgb(var(--color-green-rgb));
}

.canvas-node.is-themed.mod-canvas-color-5
  .canvas-node-content
  .markdown-preview-view
  .inline-title {
  color: rgb(var(--color-blue-rgb));
}

.canvas-node.is-themed.mod-canvas-color-6
  .canvas-node-content
  .markdown-preview-view
  .inline-title {
  color: rgb(var(--color-purple-rgb));
}

.canvas-node.is-themed.mod-canvas-color-1 .canvas-node-container,
.canvas-node.is-themed.mod-canvas-color-2 .canvas-node-container,
.canvas-node.is-themed.mod-canvas-color-3 .canvas-node-container,
.canvas-node.is-themed.mod-canvas-color-4 .canvas-node-container,
.canvas-node.is-themed.mod-canvas-color-5 .canvas-node-container,
.canvas-node.is-themed.mod-canvas-color-6 .canvas-node-container {
  border: 1px solid rgb(var(--canvas-color));
}

.theme-light .canvas-node.is-themed.mod-canvas-color-1 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(0deg 87% 79%) 0%,
    hsl(360deg 87% 78%) 21%,
    hsl(360deg 87% 77%) 30%,
    hsl(359deg 87% 75%) 39%,
    hsl(359deg 87% 74%) 46%,
    hsl(359deg 87% 73%) 54%,
    hsl(359deg 86% 72%) 61%,
    hsl(358deg 86% 71%) 69%,
    hsl(358deg 86% 70%) 79%,
    hsl(358deg 85% 68%) 100%
  );
}

.theme-dark .canvas-node.is-themed.mod-canvas-color-1 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(18deg 88% 66%) 0%,
    hsl(17deg 88% 65%) 21%,
    hsl(16deg 87% 63%) 30%,
    hsl(15deg 86% 62%) 39%,
    hsl(14deg 85% 60%) 46%,
    hsl(13deg 85% 59%) 54%,
    hsl(11deg 84% 57%) 61%,
    hsl(10deg 83% 56%) 69%,
    hsl(8deg 82% 55%) 79%,
    hsl(6deg 81% 54%) 100%
  );
}

.theme-light .canvas-node.is-themed.mod-canvas-color-2 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(16deg 100% 76%) 0%,
    hsl(20deg 100% 76%) 21%,
    hsl(23deg 100% 76%) 30%,
    hsl(27deg 100% 77%) 39%,
    hsl(30deg 100% 77%) 46%,
    hsl(34deg 100% 77%) 54%,
    hsl(37deg 100% 78%) 61%,
    hsl(41deg 100% 79%) 69%,
    hsl(45deg 100% 80%) 79%,
    hsl(49deg 100% 81%) 100%
  );
}

.theme-dark .canvas-node.is-themed.mod-canvas-color-2 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(23deg 92% 71%) 0%,
    hsl(21deg 93% 71%) 21%,
    hsl(18deg 93% 71%) 30%,
    hsl(16deg 93% 72%) 39%,
    hsl(14deg 93% 72%) 46%,
    hsl(11deg 93% 72%) 54%,
    hsl(9deg 92% 73%) 61%,
    hsl(6deg 91% 73%) 69%,
    hsl(3deg 89% 73%) 79%,
    hsl(0deg 87% 73%) 100%
  );
}

.theme-light .canvas-node.is-themed.mod-canvas-color-3 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(60deg 89% 72%) 0%,
    hsl(59deg 91% 73%) 21%,
    hsl(57deg 92% 74%) 30%,
    hsl(56deg 94% 76%) 39%,
    hsl(55deg 96% 77%) 46%,
    hsl(53deg 97% 78%) 54%,
    hsl(52deg 98% 79%) 61%,
    hsl(51deg 99% 80%) 69%,
    hsl(50deg 100% 80%) 79%,
    hsl(49deg 100% 81%) 100%
  );
}

.theme-dark .canvas-node.is-themed.mod-canvas-color-3 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(46deg 95% 56%) 0%,
    hsl(44deg 95% 55%) 21%,
    hsl(43deg 94% 54%) 30%,
    hsl(41deg 94% 53%) 39%,
    hsl(39deg 93% 53%) 46%,
    hsl(37deg 92% 53%) 54%,
    hsl(35deg 91% 52%) 61%,
    hsl(34deg 89% 52%) 69%,
    hsl(32deg 88% 52%) 79%,
    hsl(29deg 86% 52%) 100%
  );
}

.theme-light .canvas-node.is-themed.mod-canvas-color-4 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(99deg 75% 75%) 0%,
    hsl(103deg 75% 77%) 21%,
    hsl(108deg 75% 79%) 30%,
    hsl(113deg 76% 81%) 39%,
    hsl(119deg 76% 83%) 46%,
    hsl(124deg 77% 84%) 54%,
    hsl(129deg 79% 85%) 61%,
    hsl(133deg 80% 86%) 69%,
    hsl(137deg 81% 86%) 79%,
    hsl(141deg 81% 87%) 100%
  );
}

.theme-dark .canvas-node.is-themed.mod-canvas-color-4 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(145deg 84% 73%) 0%,
    hsl(145deg 78% 71%) 21%,
    hsl(146deg 74% 68%) 30%,
    hsl(146deg 70% 66%) 39%,
    hsl(146deg 67% 63%) 46%,
    hsl(147deg 64% 60%) 54%,
    hsl(148deg 61% 57%) 61%,
    hsl(148deg 60% 55%) 69%,
    hsl(149deg 58% 52%) 79%,
    hsl(150deg 61% 48%) 100%
  );
}

.theme-light .canvas-node.is-themed.mod-canvas-color-5 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(187deg 100% 89%) 0%,
    hsl(187deg 100% 87%) 21%,
    hsl(187deg 100% 85%) 30%,
    hsl(187deg 100% 83%) 39%,
    hsl(187deg 100% 81%) 46%,
    hsl(187deg 100% 79%) 54%,
    hsl(187deg 100% 77%) 61%,
    hsl(186deg 100% 75%) 69%,
    hsl(186deg 100% 72%) 79%,
    hsl(186deg 100% 69%) 100%
  );
}

/* .theme-light .canvas-node.is-themed.mod-canvas-color-5 .canvas-node-content p{
	color: white;
} */

.theme-dark .canvas-node.is-themed.mod-canvas-color-1 .canvas-node-content p,
.theme-dark .canvas-node.is-themed.mod-canvas-color-2 .canvas-node-content p,
.theme-dark .canvas-node.is-themed.mod-canvas-color-3 .canvas-node-content p,
.theme-dark .canvas-node.is-themed.mod-canvas-color-4 .canvas-node-content p,
.theme-dark .canvas-node.is-themed.mod-canvas-color-5 .canvas-node-content p,
.theme-dark .canvas-node.is-themed.mod-canvas-color-6 .canvas-node-content p {
  color: var(--text-on-accent);
}

.theme-dark .canvas-node.is-themed.mod-canvas-color-5 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(210deg 90% 80%) 0%,
    hsl(211deg 91% 77%) 21%,
    hsl(212deg 92% 74%) 30%,
    hsl(212deg 93% 71%) 39%,
    hsl(213deg 93% 68%) 46%,
    hsl(213deg 93% 65%) 54%,
    hsl(213deg 92% 61%) 61%,
    hsl(213deg 91% 58%) 69%,
    hsl(213deg 90% 54%) 79%,
    hsl(212deg 93% 49%) 100%
  );
}

.theme-light .canvas-node.is-themed.mod-canvas-color-6 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(298deg 68% 90%) 0%,
    hsl(287deg 68% 89%) 21%,
    hsl(277deg 68% 89%) 30%,
    hsl(267deg 67% 88%) 39%,
    hsl(258deg 65% 87%) 46%,
    hsl(249deg 63% 87%) 54%,
    hsl(240deg 61% 86%) 61%,
    hsl(232deg 62% 83%) 69%,
    hsl(225deg 62% 81%) 79%,
    hsl(220deg 61% 79%) 100%
  );
}

.theme-dark .canvas-node.is-themed.mod-canvas-color-6 .canvas-node-content {
  background-image: linear-gradient(
    45deg,
    hsl(276deg 91% 79%) 0%,
    hsl(274deg 88% 77%) 21%,
    hsl(272deg 85% 75%) 30%,
    hsl(270deg 83% 74%) 39%,
    hsl(267deg 81% 72%) 46%,
    hsl(265deg 79% 71%) 54%,
    hsl(262deg 78% 69%) 61%,
    hsl(260deg 76% 68%) 69%,
    hsl(257deg 75% 66%) 79%,
    hsl(254deg 74% 65%) 100%
  );
}
```
