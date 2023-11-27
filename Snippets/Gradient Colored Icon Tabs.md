↪[Collection](Collection.md)

# Gradient Colored Icon Tabs

---

- author:: ebullient
- source:: https://discord.com/channels/686053708261228577/702656734631821413/930097778741354517

---

> _Only works when your note is on one of the sidebars. You can change file name `colors` in the code with your file name_

cover:: ![](https://i.imgur.com/JDNmpNe.png)

```css
/*
author: ebullient
source: https://discord.com/channels/686053708261228577/702656734631821413/930097778741354517
*/

.workspace-tab-header[aria-label="colors"]
  > .workspace-tab-header-inner
  > .workspace-tab-header-inner-icon {
  width: 17px;
  height: 17px;
  background: red; /* For browsers that do not support gradients */
  background: -webkit-linear-gradient(
    left,
    red,
    orange,
    yellow,
    green,
    cyan,
    blue,
    violet
  ); /* For Safari 5.1 to 6.0 */
  background: -o-linear-gradient(
    right,
    red,
    orange,
    yellow,
    green,
    cyan,
    blue,
    violet
  ); /* For Opera 11.1 to 12.0 */
  background: -moz-linear-gradient(
    right,
    red,
    orange,
    yellow,
    green,
    cyan,
    blue,
    violet
  ); /* For Firefox 3.6 to 15 */
  background: linear-gradient(
    to right,
    red,
    orange,
    yellow,
    green,
    cyan,
    blue,
    violet
  ); /* Standard syntax (must be last) */
  border-radius: 4px;
}
.workspace-tab-header[aria-label="colors"]
  > .workspace-tab-header-inner
  > .workspace-tab-header-inner-icon
  > svg {
  display: none;
}
```

---
