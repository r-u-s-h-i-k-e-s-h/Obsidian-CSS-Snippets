↪[Collection](Collection.md)

# Top Backlinks

---

- author:: ThisTheThe
- source:: https://github.com/ThisTheThe/MicroMike

#MicroMike 

---

To try it out: Enable the snippet "sTopBacklinks".

cover:: ![](https://i.imgur.com/VG2a46u.png) 

```
@charset "UTF-8";
/* 
	Top Backlinks
	Toplinks (I.E. LYT/Ideaverse) are obnoxious to manually maintain. This snippet turns the backlinks's panel at the bottom into an autommatic "Toplinks" section.
*/
/*
	Author: ThisTheThe
	Source: github.com/ThisTheThe/MicroMike
	Version: 03/11/2025
	This is a componentized version of a portion of Micro Mike. 
	If you like what you see here, you might like the theme.

	Feel free to give feedback on the theme page, or on Discord - I can be reached at "liblung". 
*/
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) {
  display: flex;
  flex-direction: column;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) {
  padding: 0px;
  margin: 0px;
  border: 0px;
  gap: 0px;
  order: -1;
  min-height: unset !important;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer):has(> .backlink-pane > .search-result-container > .search-empty-state) {
  display: none;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .nav-header {
  display: none;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane > .tree-item-self {
  display: none;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container {
  padding: 0px;
  margin: 0px;
  gap: 0px;
  padding-bottom: 10px;
  border-bottom: 2px solid var(--hr-color);
  margin-bottom: 10px;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children {
  display: flex;
  flex-wrap: wrap;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result {
  display: flex;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-matches {
  display: none;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-title.tree-item-self.is-clickable:hover {
  background-color: transparent;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-title.tree-item-self.is-clickable .tree-item-icon {
  display: none;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-title.tree-item-self.is-clickable .tree-item-flair-outer {
  display: none;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-title.tree-item-self.is-clickable .tree-item-inner {
  line-height: 35px;
  font-size: var(--font-text-size);
  white-space: nowrap;
  color: var(--link-color);
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-title.tree-item-self.is-clickable .tree-item-inner:hover {
  color: var(--link-color-hover);
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-title.tree-item-self.is-clickable .tree-item-inner:hover::before {
  text-decoration-line: none;
  text-decoration: none;
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-title.tree-item-self.is-clickable .tree-item-inner::before {
  content: "႟";
  color: var(--text-normal);
}
:not(.disableToplinks) :is(.markdown-reading-view, .markdown-source-view) :is(.markdown-preview-sizer, .cm-sizer) :is(.embedded-backlinks, .mod-footer) .backlink-pane .search-result-container .search-results-children .search-result .search-result-file-title.tree-item-self.is-clickable .tree-item-inner::after {
  content: "";
  color: var(--text-normal);
}/*# sourceMappingURL=sTopBacklinks.css.map */
```