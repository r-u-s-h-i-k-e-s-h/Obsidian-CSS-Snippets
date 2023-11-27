↪[Collection](Collection.md)

# Image gallery

---

- author:: WindWalker
- source:: https://discord.com/channels/686053708261228577/744933215063638183/1098803015164633139

---

cover:: ![](https://i.imgur.com/heTNDVW.gif)

```css
/*
author: WindWalker
source: https://discord.com/channels/686053708261228577/744933215063638183/1098803015164633139
*/

/* Adjustable Hight, Manual Width Aadjustment*/

    body .imagegallery {
    --file-line-width: 1100px;
  }


    .imagegallery .cm-editor img {
      max-width: 300px;
    }

    .imagegallery p {
        display: flex;
        flex-wrap: wrap;
        justify-content: flex-start;
        align-content: flex-start;
    }

    .imagegallery p span {
        margin: 5px;
        border: 0px solid #ccc;
        height: 250px;
    }

    .imagegallery p img {
      height: 250px;
      object-fit: cover;
      transition: .0s;
    }

    .imagegallery p img:hover {
      object-fit: cover;
      /*box-shadow: 5px 5px 15px rgb(0, 0, 0, 0.5);*/
    }


    .imagegallery p span:hover img:not(:active) {
      transition: transform .1s ;
      transition-property: ;
      transform: scale(1.13);
      z-index: 1000;
      transition-property: initial;
      box-shadow: 5px 5px 10px rgb(0, 0, 0, 0.4);

    }


    .popover .imagegallery img {
      width: 100px;
      height: 100px;
    }

    .popover .imagegallery p span {
    width: 100px;
    height: 100px;
    }

    .popover .imagegallery p span:hover img:not(:active) {
      transform: scale(1.05);
    }

    .imagegallery p img:active{
    transition: none;
    display:block;
    z-index:100;
    position:fixed;
    max-height:100%;
    max-width:100%;
    height:100%;
    width:100%;
    object-fit: contain;
    margin:0 auto;
    text-align:center;
    top: 50%;
    transform: translateY(-50%);
    padding:0;
    left:0;
    right:0;
    bottom:0;
    background:var(--background-primary);}
    }


/*
    body .imagegallery {
    --file-line-width: 1120px;
  }

    .imagegallery p {
        display: flex;
        flex-wrap: wrap;
        justify-content: flex-start;
        align-content: flex-start;
    }

    .imagegallery p span {
        margin: 6px;
        margin-bottom: -2px;
        border: 0px solid #ccc;
        height: auto;
    }

    .imagegallery p img {
      max-height: 175px;
      padding: 0px;
      object-fit: cover;
    }


    .imagegallery p span:hover {

    }
*/
```

---

## How to use

```md
---
cssclasses:
  - imagegallery
---

![[image 01.jpg]]
![[image 01.jpg]]
![[image 01.jpg]]
![[image 01.jpg]]
```
