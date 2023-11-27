↪[Collection](Collection.md)

# External link styling 01

---

- author:: sailKite
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1144453260707647538

---

cover:: ![](https://i.imgur.com/WzApq7M.png)

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1144453260707647538
*/

.external-link:after {
  content: "";
  display: inline-block;
  font-weight: 300;
  font-size: 15px;
  margin-left: 2px;
  transition: 100ms;

  /* these bits are for sizing the box */
  width: 1em;
  aspect-ratio: 1;

  /* setting the "image" as a mask through which the background color can show */
  -webkit-mask-image: url("data:image/svg+xml,%3Csvg xmlns='http://www.w3.org/2000/svg' stroke='currentColor' fill='currentColor' viewBox='0 0 24 24'%3E%3Cpath d='M18.3643 15.5353L16.95 14.1211L18.3643 12.7069C20.3169 10.7543 20.3169 7.58847 18.3643 5.63585C16.4116 3.68323 13.2458 3.68323 11.2932 5.63585L9.87898 7.05007L8.46477 5.63585L9.87898 4.22164C12.6127 1.48797 17.0448 1.48797 19.7785 4.22164C22.5121 6.95531 22.5121 11.3875 19.7785 14.1211L18.3643 15.5353ZM15.5358 18.3638L14.1216 19.778C11.388 22.5117 6.9558 22.5117 4.22213 19.778C1.48846 17.0443 1.48846 12.6122 4.22213 9.87849L5.63634 8.46428L7.05055 9.87849L5.63634 11.2927C3.68372 13.2453 3.68372 16.4112 5.63634 18.3638C7.58896 20.3164 10.7548 20.3164 12.7074 18.3638L14.1216 16.9496L15.5358 18.3638ZM14.8287 7.75717L16.2429 9.17139L9.17187 16.2425L7.75766 14.8282L14.8287 7.75717Z'%3E%3C/path%3E%3C/svg%3E");
  background-color: currentColor;
}

/* remove external link icon */
.external-link {
  background-image: none;
  padding-right: 0;
}
```
