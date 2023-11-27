↪[Collection](Collection.md)

# Banner

---

- author:: KuiyueRO
- source:: https://github.com/KuiyueRO/Obsidian-Miner/blob/main/snippets/MinerBanner.css
- guide:: https://github.com/KuiyueRO/Obsidian-Miner/blob/main/md/MinerBanner.md

---

cover:: ![](https://i.imgur.com/Fe9ACem.jpg)

```css
/*
MIT License

Copyright (c) 2023 KuiyueRO

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
*/

/*
Author: KuiyueRO
URL: https://github.com/KuiyueRO/Obsidian-Miner/edit/main/snippets/MinerBanner.css

==A CSS snippets to show your banner and banner icon for obsidian.==

Style Setting Support: WIP

Wikilink only:
banner image: √
banner image icon: √
banner text icon: ×
banner emoji icon: ×
description: ×

Callout: (Best)
banner image: √
banner image icon: √
banner text icon: √
banner emoji icon: √
description: √

dataview inline field: (Huawei Webview doesn't support :has(), so abandon it)
banner image: ×
banner image icon: ×
banner text icon: √
banner emoji icon: √
description: √

*/

body {
  --bannericon-wh: 5em;
  --bannericon-top: 5.5em;
  --bannerimg-height: 11em;
  --bannericon-circle-radius: 5em;
  --bannericon-square-radius: 0.75em;
  --bannericon-border-width: 0.175em;
}

.markdown-reading-view .bannerimg {
  padding-bottom: 2em !important;
  padding-top: var(--bannerimg-height) !important;
}

.canvas-node-content.markdown-embed .bannerimg {
  padding-top: 11em !important;
}

span[src$="bannerimg"] img {
  top: 0;
  left: 0;
  z-index: 9;
  width: 100%;
  max-width: 100%;
  margin-top: 0px;
  max-height: 10em;
  min-height: 10em;
  object-fit: cover;
  border-radius: 0px;
  position: absolute;
}

span[src$="bannericonl"] img,
span[src$="bannericonlc"] img,
span[src$="bannericonc"] img,
span[src$="bannericoncc"] img {
  top: var(--bannericon-top);
  width: var(--bannericon-wh) !important;
  height: var(--bannericon-wh) !important;
  z-index: 9;
  object-fit: cover;
  position: absolute;
  box-shadow: var(--shadow-l);
  background-color: var(--background-secondary-alt);
  border: var(--bannericon-border-width) solid var(--background-secondary-alt);
}

span[src$="bannericonl"] img {
  left: var(--h1-style);
  border-radius: var(--bannericon-square-radius) !important;
}

span[src$="bannericonlc"] img {
  left: initial;
  border-radius: var(--bannericon-circle-radius) !important;
}

span[src$="bannericonc"] img {
  left: calc(50% - 2.5em);
  border-radius: var(--bannericon-square-radius) !important;
}

span[src$="bannericoncc"] img {
  left: calc(50% - 2.5em);
  border-radius: var(--bannericon-circle-radius) !important;
}

/*=======Title Align Center=======*/
.banner-title-center .inline-title {
  text-align: center !important;
}

/*=======CallOut Support=======*/
/*Banner Image*/
.callout[data-callout="bannerimage"] .callout-content {
  top: 0;
  left: 0;
  height: 10em;
  display: flex;
  padding: unset;
  overflow: clip;
  position: absolute;
  align-items: center;
  object-fit: inherit !important;
}

.callout[data-callout="bannerimage"] .callout-content > p,
.callout[data-callout="bannerimage"] .callout-content > p > span {
  margin: unset;
  object-fit: inherit;
}

.callout[data-callout="bannerimage"] .callout-content > p > span > img {
  margin: unset;
  width: 1000000em !important;
  height: 10em;
  object-fit: cover;
}

/*Description left and Description center*/
.description
  .markdown-preview-sizer.markdown-preview-section
  > .mod-header
  > .inline-title {
  margin-bottom: calc(5 * var(--inline-title-margin-bottom));
}

.markdown-reading-view
  .callout[data-callout="bannerdescription"]
  .callout-content {
  top: 13.55em;
  overflow: hidden;
  position: absolute;
  left: var(--h1-style);
  border-left: var(--h1-style) solid;
}

.canvas .callout[data-callout="bannerdescription"] .callout-content {
  top: 13.55em;
  overflow: hidden;
  /*position: absolute;*/
  left: var(--h1-style);
  border-left: var(--h1-style) solid;
}

.canvas .callout[data-callout="bannerdescriptionc"] .callout-content {
  left: 0;
  top: 13.55em;
  overflow: hidden;
  /*position: absolute;*/
  border-left: var(--h1-style) solid;
}

.callout[data-callout="bannerdescription"] .callout-content > p {
  padding-top: 8px;
  font-size: var(--size-4-3);
  color: var(--color-base-60);
  height: calc(var(--size-4-4) * 2);
  text-overflow: ellipsis !important;
  border-top: 2px solid var(--color-base-100);
  margin-right: calc(var(--file-margins) * 2);
  border-image: linear-gradient(
      to right,
      var(--color-base-100),
      var(--color-base-00)
    ) 1;
}

.markdown-reading-view
  .callout[data-callout="bannerdescriptionc"]
  .callout-content
  > p,
.canvas .callout[data-callout="bannerdescriptionc"] .callout-content > p {
  padding-top: 8px;
  text-align: center;
  font-size: var(--size-4-3);
  color: var(--color-base-60);
  height: calc(var(--size-4-4) * 2);
  text-overflow: ellipsis !important;
  border-top: 2px solid var(--color-base-100);
  border-image: linear-gradient(
      to right,
      var(--color-base-00),
      var(--color-base-100),
      var(--color-base-00)
    ) 1;
}

.markdown-reading-view
  .callout[data-callout="bannerdescriptionc"]
  .callout-content
  > p {
  width: 100% !important;
}

.markdown-reading-view
  .callout[data-callout="bannerdescriptionc"]
  .callout-content {
  position: absolute;
  left: 0;
  top: 13.55em;
  padding-left: var(--file-margins) !important;
  padding-right: var(--file-margins) !important;
  overflow: hidden;
}

/*Left square Icon*/
.callout[data-callout="bannericonl"] .callout-content {
  top: 5.5em;
  overflow: visible;
  position: absolute;
  left: var(--h1-style);
}

.callout[data-callout="bannericonl"] .callout-content > p {
  display: flex;
  font-size: 5em;
  aspect-ratio: 1;
  position: relative;
  align-items: center;

  justify-content: center;
  border: unset !important;
  width: calc(var(--bannericon-wh) / 5);
  height: calc(var(--bannericon-wh) / 5);
  margin: unset;
  object-fit: inherit;
}

.callout[data-callout="bannericonl"] .callout-content > p > span > img {
  display: flex;
  aspect-ratio: 1;
  box-shadow: var(--shadow-l);
  font-size: var(--font-text-size);
  overflow: hidden;
  object-fit: cover;
  background-color: var(--background-secondary-alt);
  border: var(--bannericon-border-width) solid var(--background-secondary-alt);
  left: var(--h1-style);
  border-radius: var(--bannericon-square-radius) !important;
}

/* Left Circle Icon*/
.callout[data-callout="bannericonlc"] .callout-content {
  top: 5.5em;
  overflow: visible;
  position: absolute;
  left: var(--h1-style);
}

.callout[data-callout="bannericonlc"] .callout-content > p {
  display: flex;
  font-size: 5em;
  aspect-ratio: 1;
  position: relative;
  align-items: center;

  justify-content: center;
  border: unset !important;
  width: calc(var(--bannericon-wh) / 5);
  height: calc(var(--bannericon-wh) / 5);
  margin: unset;
  object-fit: inherit;
}

.callout[data-callout="bannericonlc"] .callout-content > p > span > img {
  display: flex;
  aspect-ratio: 1;
  box-shadow: var(--shadow-l);
  font-size: var(--font-text-size);
  overflow: hidden;
  object-fit: cover;
  background-color: var(--background-secondary-alt);
  border: var(--bannericon-border-width) solid var(--background-secondary-alt);
  border-radius: var(--bannericon-circle-radius) !important;
  left: var(--h1-style);
}

/*Center square Icon*/
.callout[data-callout="bannericonc"] .callout-content {
  top: 5.5em;
  display: flex;
  overflow: visible;
  position: absolute;
  left: calc(50% - 2.5em);
}

.callout[data-callout="bannericonc"] .callout-content > p {
  display: flex;
  font-size: 5em;
  aspect-ratio: 1;
  position: relative;
  align-items: center;

  justify-content: center;
  border: unset !important;
  width: calc(var(--bannericon-wh) / 5);
  height: calc(var(--bannericon-wh) / 5);
  margin: unset;
  object-fit: inherit;
}

.callout[data-callout="bannericonc"] .callout-content > p > span > img {
  display: flex;
  aspect-ratio: 1;
  box-shadow: var(--shadow-l);
  font-size: var(--font-text-size);
  overflow: hidden;
  object-fit: cover;
  background-color: var(--background-secondary-alt);
  border: var(--bannericon-border-width) solid var(--background-secondary-alt);
  left: var(--h1-style);
  border-radius: var(--bannericon-square-radius) !important;
}

/*Center Circle Icon*/
.callout[data-callout="bannericoncc"] .callout-content {
  top: 5.5em;
  overflow: visible;
  position: absolute;
  left: calc(50% - 40px);
}

.callout[data-callout="bannericoncc"] .callout-content > p {
  display: flex;
  font-size: 5em;
  aspect-ratio: 1;
  position: relative;
  align-items: center;

  justify-content: center;
  border: unset !important;
  width: calc(var(--bannericon-wh) / 5);
  height: calc(var(--bannericon-wh) / 5);
  margin: unset;
  object-fit: inherit;
}

.callout[data-callout="bannericoncc"] .callout-content > p > span > img {
  display: flex;
  aspect-ratio: 1;
  box-shadow: var(--shadow-l);
  font-size: var(--font-text-size);
  overflow: hidden;
  object-fit: cover;
  background-color: var(--background-secondary-alt);
  border: var(--bannericon-border-width) solid var(--background-secondary-alt);
  border-radius: var(--bannericon-circle-radius) !important;
  left: var(--h1-style);
}

/*Hide Default CallOut Style*/
.callout[data-callout="banner"] .callout-title,
.callout[data-callout="banner"] .callout-icon,
.callout[data-callout="banner"] .callout-icon::after,
.callout[data-callout="banner"] .callout-fold,
.callout[data-callout="bannerimage"] .callout-title,
.callout[data-callout="bannerimage"] .callout-icon,
.callout[data-callout="bannerimage"] .callout-icon::after,
.callout[data-callout="bannerimage"] .callout-fold,
.callout[data-callout="bannerdescription"] .callout-title,
.callout[data-callout="bannerdescription"] .callout-icon,
.callout[data-callout="bannerdescription"] .callout-icon::after,
.callout[data-callout="bannerdescription"] .callout-fold,
.callout[data-callout="bannerdescriptionc"] .callout-title,
.callout[data-callout="bannerdescriptionc"] .callout-icon,
.callout[data-callout="bannerdescriptionc"] .callout-icon::after,
.callout[data-callout="bannerdescriptionc"] .callout-fold,
.callout[data-callout="bannericonl"] .callout-title,
.callout[data-callout="bannericonl"] .callout-icon,
.callout[data-callout="bannericonl"] .callout-icon::after,
.callout[data-callout="bannericonl"] .callout-fold,
.callout[data-callout="bannericonlc"] .callout-title,
.callout[data-callout="bannericonlc"] .callout-icon,
.callout[data-callout="bannericonlc"] .callout-icon::after,
.callout[data-callout="bannericonlc"] .callout-fold,
.callout[data-callout="bannericonc"] .callout-title,
.callout[data-callout="bannericonc"] .callout-icon,
.callout[data-callout="bannericonc"] .callout-icon::after,
.callout[data-callout="bannericonc"] .callout-fold,
.callout[data-callout="bannericoncc"] .callout-title,
.callout[data-callout="bannericoncc"] .callout-icon,
.callout[data-callout="bannericoncc"] .callout-icon::after,
.callout[data-callout="bannericoncc"] .callout-fold {
  display: none;
}

.callout[data-callout="bannericonl"],
.callout[data-callout="bannericonlc"],
.callout[data-callout="bannericonc"],
.callout[data-callout="bannericoncc"],
.callout[data-callout="banner"],
.callout[data-callout="bannerdescription"],
.callout[data-callout="bannerdescriptionc"],
.callout[data-callout="bannerimage"] {
  width: 100%;
  margin: unset;
  padding: unset;
  border-style: unset;
  border-color: unset;
  border-width: unset;
  border-radius: unset;
  mix-blend-mode: unset;
  background-color: unset;
  overflow: visible !important;
}

.callout[data-callout="bannerimage"] {
  display: flex;
  align-items: center;
  width: auto !important;
  object-fit: cover !important;
}

.callout[data-callout="bannerdescription"],
.callout[data-callout="bannerdescriptionc"] {
  top: 20em;
}

/*=======Plugin Support=======*/
/*Strange New World*/
.snw-reference[data-snw-reallink$="bannerimg"],
.snw-reference[data-snw-reallink*="bannericon"] {
  display: none !important;
}

/*Breadcrumbs*/
.bannerimg .BC-trail,
.bannericon .BC-trail {
  padding: 5px;
  border-radius: 5px;
  margin-top: 1.5em !important;
  border: 1px solid var(--background-modifier-border);
}

.bannerimg
  .BC-trail
  .markdown-reading-view
  > .markdown-preview-view.is-readable-line-width,
.markdown-source-view.is-readable-line-width .cm-sizer {
  padding-top: unset;
}

/*Canvas*/
.canvas-node-content.markdown-embed
  > .markdown-embed-content
  > .markdown-preview-view:has([alt*="bannerimg"])::before {
  content: unset !important;
}

.canvas
  .description
  .markdown-preview-sizer.markdown-preview-section
  > .mod-header
  > .inline-title {
  margin-bottom: unset;
}

.canvas-node-content.markdown-embed
  > .markdown-embed-content
  > .markdown-preview-view::before,
.canvas-node-content.markdown-embed
  > .markdown-embed-content
  > .markdown-preview-view::after {
  content: none;
  display: block;
}

.canvas .callout[data-callout="bannerdescriptionc"] .callout-content > p {
  margin-left: calc(var(--file-margins));
  margin-right: calc(var(--file-margins));
}
```
