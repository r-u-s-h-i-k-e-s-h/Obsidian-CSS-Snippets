---
author: TheMathGuyd
source: https://discord.com/channels/686053708261228577/702656734631821413/1254526461994602567
cover: "[[gif-link styling (external) - squiggly effect on hover.gif]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Link styling (external) - squiggly effect on hover

![](../attachments/gif-link%20styling%20(external)%20-%20squiggly%20effect%20on%20hover.gif)

## Snippet

```css
/*
author: TheMathGuyd
source: https://discord.com/channels/686053708261228577/702656734631821413/1254526461994602567
*/

.external-link:hover {
  color: var(--accent-4);
  background-image: url("data:image/svg+xml;charset=utf8,%3Csvg id=%27squiggle-link%27 xmlns=%27http://www.w3.org/2000/svg%27 xmlns:xlink=%27http://www.w3.org/1999/xlink%27 xmlns:ev=%27http://www.w3.org/2001/xml-events%27 viewBox=%270 0 10 18%27%3E%3Cstyle type=%27text/css%27%3E.squiggle{animation:shift .5s linear infinite;}@keyframes shift {from {transform:translateX%28-10px%29;}to {transform:translateX%280%29;}}%3C/style%3E%3Cpath fill=%27none%27 stroke=%27%23FFEF00%27 stroke-width=%270.5%27 class=%27squiggle%27 d=%27M0,17.5 c 2.5,0,2.5,-1.5,5,-1.5 s 2.5,1.5,5,1.5 c 2.5,0,2.5,-1.5,5,-1.5 s 2.5,1.5,5,1.5%27 /%3E%3C/svg%3E");
  background-position: 0 100%;
  background-size: auto 36px;
  background-repeat: repeat;
  text-decoration: none;
  border-bottom: none;
  padding-bottom: 3px;
  word-break: break-word;
}
```
