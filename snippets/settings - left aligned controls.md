---
author: ThisTheThe
source: https://github.com/ThisTheThe/MicroMike
cover: "[[img-settings - left aligned controls.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Settings - left aligned controls

![](../attachments/img-settings%20-%20left%20aligned%20controls.webp)

## Snippet

```css
/*
	Left Aligned Settings Controls
	This makes interactable elements in the settings menu left-aligned, pushing against the text.
	It makes it much clearer which interactable belongs to which setting, and elegantly sectionally divides the window.
*/
/*
	Author: ThisTheThe
	Source: github.com/ThisTheThe/MicroMike
	Version: 03/11/2025
	This is a componentized version of a portion of Micro Mike.
	If you like what you see here, you might like the theme.

	Feel free to give feedback on the theme page, or on Discord - I can be reached at "liblung".
*/
body {
  --settingsLeftColumnLength: 200px;
}

/* @settings
name: Left Aligned Settings Controls
id: ScrollBar
settings:
	-
		id: settingsLeftColumnLength
		title: Left Column Width
		description: The width of the controls' column.
		type: variable-number-slider
		default: 200
		min: 150
		max: 350
		step: 2
		format: px
*/
body:not(.disableLeftAlignSettings):not(.is-mobile) .modal.mod-settings .vertical-tab-content:not(.file-explorer-plus) .setting-item-control {
  order: -1;
  flex-grow: 0;
  flex-shrink: 0;
  min-width: var(--settingsLeftColumnLength);
  margin-right: 10px;
  max-width: var(--settingsLeftColumnLength);
  flex-wrap: wrap;
}

body:not(.disableLeftAlignSettings):not(.is-mobile) .modal.mod-settings .vertical-tab-content:not(.file-explorer-plus) .setting-item-control .dropdown,
body:not(.disableLeftAlignSettings):not(.is-mobile) .modal.mod-settings .vertical-tab-content:not(.file-explorer-plus) .setting-item-control .search-input-container {
  text-wrap: wrap;
  max-width: var(--settingsLeftColumnLength);
  height: initial;
  padding-top: 5px;
  padding-bottom: 5px;
  display: flex;
}

body:not(.disableLeftAlignSettings):not(.is-mobile) .modal.mod-settings .vertical-tab-content:not(.file-explorer-plus) .setting-item-control textarea {
  max-width: var(--settingsLeftColumnLength);
}

/*# sourceMappingURL=sLeftAlignSettingsControls.css.map */
```
