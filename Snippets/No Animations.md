↪[Collection](Collection.md)

# No Animations

---

- author:: ThisTheThe
- source:: https://github.com/ThisTheThe/MicroMike

#MicroMike 

---

To try it out: Enable the snippet "sNoAnimation".

cover:: ![](https://i.imgur.com/Lk18z4F.png) 

```
/* 
	No Animations
	This snippet disables animations. It includes a feature to workaround a problem causing the sidebars to close more slowly, and a fix for issues with the file browser display.
*/
/*
	Author: ThisTheThe
	Source: github.com/ThisTheThe/MicroMike
	Version: 03/10/2025
	This is a componentized version of a portion of Micro Mike. 
	If you like what you see here, you might like the theme.

	Feel free to give feedback on the theme page, or on Discord - I can be reached at "liblung". 
*/
/* Animation Disabler */
*, *:after, *:before {
  /*CSS transitions*/
  transition-property: none !important;
  transition: none !important;
  /*CSS transforms*/
  /*CSS animations*/
  animation: none !important;
}

body .workspace-split.mod-horizontal.mod-left-split.is-sidedock-collapsed {
  display: none !important;
}

body .workspace-split.mod-horizontal.mod-right-split.is-sidedock-collapsed {
  display: none !important;
}

.workspace-leaf-content {
  animation: 0.03s fade cubic-bezier(0.25, 0.46, 0.45, 0.94) !important;
}
```