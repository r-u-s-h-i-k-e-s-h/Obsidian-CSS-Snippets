↪[Collection](Collection.md)

# Image styling - Zoom image

---

- author:: Kepano
- source:: https://forum.obsidian.md/t/image-zoom-click-hold-to-expand-images/5164?u

---

cover:: ![](https://i.imgur.com/ObcCIWz.gif)

```css
/*
author: Kepano
source: https://forum.obsidian.md/t/image-zoom-click-hold-to-expand-images/5164?u
*/

.view-content img {
  max-width: 100%;
  cursor: zoom-in;
}

.view-content img:active {
  cursor: zoom-out;
}
.view-content .markdown-preview-view img[referrerpolicy="no-referrer"]:active,
.view-content .image-embed:active {
  background: var(--background-primary);
  cursor: zoom-out;
  display: block;
  z-index: 200;
  position: fixed;
  max-height: 100%;
  max-width: 100%;
  height: 100%;
  width: 100%;
  object-fit: contain;
  margin: 0 auto;
  text-align: center;
  padding: 0;
  left: 0;
  right: 0;
  bottom: 0;
}
.view-content .image-embed:active img {
  top: 50%;
  transform: translateY(-50%);
  padding: 0;
  margin: 0 auto;
  width: 100%;
  max-height: 100vh;
  object-fit: contain;
  left: 0;
  right: 0;
  bottom: 0;
  position: absolute;
  opacity: 1;
}
```
