↪[Collection](Collection.md)

# Callout styling - Old callouts

---

- author:: kepano
- source:: https://gist.github.com/kepano/cde61ac7db1afd3f173a16157c627f93

---

cover:: ![](https://i.imgur.com/yQy1Vem.png)

```css
/*
author: kepano
source: https://gist.github.com/kepano/cde61ac7db1afd3f173a16157c627f93
*/

body {
  --callout-border-width: 0 0 0 4px;
  --callout-border-opacity: 1;
  --callout-radius: 0;
  --callout-padding: 0;
  --callout-title-padding: var(--size-4-4) var(--size-4-4);
  --callout-content-padding: var(--size-4-2) var(--size-4-4);
}
.callout-title-inner {
  color: var(--text-normal);
}
.callout-content {
  background-color: var(--background-primary-alt);
}
```
