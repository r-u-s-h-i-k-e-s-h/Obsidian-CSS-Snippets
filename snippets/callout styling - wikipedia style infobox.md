---
author: HMA-Awan
source: https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets/issues/19
cover: "[[img-callout styling - wikipedia style infobox.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Callout styling - wikipedia style infobox

> Best viewed in **Reading Mode**

![](../attachments/img-callout%20styling%20-%20wikipedia%20style%20infobox.webp)

## Snippet

```css
/*
author: HMA-Awan
source: https://github.com/r-u-s-h-i-k-e-s-h/Obsidian-CSS-Snippets/issues/19
*/

/* ========================================
   PART 1: BASE STYLES
   ======================================== */

/* ---- Sidebar Container ---- */
.callout[data-callout^="right-sidebar-"],
.callout[data-callout="right-sidebar"] {
  float: right;
  clear: right;
  width: 280px;
  margin: 0 0 1.2em 1.8em;
  padding: 0.4em 0.8em 0.2em 0.8em;
  background: var(--sidebar-bg, var(--background-secondary));
  border: 1px solid var(--sidebar-border, var(--background-modifier-border));
  border-radius: 4px;
  font-size: 0.82em;
  line-height: 1.4;
  max-height: none;
  overflow: visible;
  position: sticky;
  top: 1em;
}

/* ---- Main Title ---- */
.callout[data-callout^="right-sidebar-"] .callout-title,
.callout[data-callout="right-sidebar"] .callout-title {
  font-weight: 700;
  font-size: 1.2em;
  text-align: center;
  border-bottom: 1px solid var(--sidebar-border, var(--background-modifier-border));
  padding-bottom: 0.15em;
  margin-bottom: 0.2em;
  color: var(--text-normal) !important;
}

/* ---- Hide Default Icons ---- */
.callout[data-callout^="right-sidebar-"] .callout-icon,
.callout[data-callout="right-sidebar"] .callout-icon {
  display: none;
}

/* ========================================
   PART 2: NESTED GROUPS
   ======================================== */

/* ---- Group Container ---- */
.callout[data-callout^="right-sidebar-"] .callout[data-callout="sidebar-group"],
.callout[data-callout="right-sidebar"] .callout[data-callout="sidebar-group"] {
  margin: 0.2em 0;
  padding: 0;
  background: transparent;
  border: none;
  border-left: 2px solid var(--sidebar-border, var(--background-modifier-border));
}

/* ---- Group Heading ---- */
.callout[data-callout^="right-sidebar-"] .callout[data-callout="sidebar-group"] .callout-title,
.callout[data-callout="right-sidebar"] .callout[data-callout="sidebar-group"] .callout-title {
  font-weight: 600;
  font-size: 1.1em;
  border-bottom: none;
  padding: 0.08em 0.4em;
  margin: 0 0 0.02em 0;
  background: var(--sidebar-heading-bg, var(--background-secondary-alt));
  border-radius: 2px;
  color: var(--text-normal) !important;
}

/* ---- Hide Group Icons ---- */
.callout[data-callout^="right-sidebar-"] .callout[data-callout="sidebar-group"] .callout-icon,
.callout[data-callout="right-sidebar"] .callout[data-callout="sidebar-group"] .callout-icon {
  display: none;
}

/* ---- Group Content (Tight Spacing) ---- */
.callout[data-callout^="right-sidebar-"] .callout[data-callout="sidebar-group"] .callout-content,
.callout[data-callout="right-sidebar"] .callout[data-callout="sidebar-group"] .callout-content {
  padding: 0.02em 0 0.02em 0.4em !important;
  margin: 0 !important;
}

/* ---- Remove Extra Spacing Inside Content ---- */
.callout[data-callout^="right-sidebar-"] .callout[data-callout="sidebar-group"] .callout-content>*,
.callout[data-callout="right-sidebar"] .callout[data-callout="sidebar-group"] .callout-content>* {
  margin-top: 0 !important;
  margin-bottom: 0 !important;
  padding-top: 0 !important;
  padding-bottom: 0 !important;
}

/* ---- Link Separator ---- */
.callout[data-callout^="right-sidebar-"] .internal-link:not(:last-child)::after,
.callout[data-callout="right-sidebar"] .internal-link:not(:last-child)::after {
  content: " · ";
  color: var(--text-muted);
}

/* ========================================
   PART 3: COLOR SCHEMES
   Only Background & Border Colors Change
   Text Colors Come From Global Theme
   ======================================== */

/* ---- Default (Theme-based) ---- */
.callout[data-callout="right-sidebar"] {
  --sidebar-bg: var(--background-secondary);
  --sidebar-border: var(--background-modifier-border);
  --sidebar-heading-bg: var(--background-secondary-alt);
}

/* ---- Red ---- */
.callout[data-callout="right-sidebar-red"] {
  --sidebar-bg: #fdf2f2;
  --sidebar-border: #f5c6cb;
  --sidebar-heading-bg: rgba(220, 53, 69, 0.12);
}

/* ---- Green ---- */
.callout[data-callout="right-sidebar-green"] {
  --sidebar-bg: #f0fdf4;
  --sidebar-border: #b7e4c7;
  --sidebar-heading-bg: rgba(40, 167, 69, 0.12);
}

/* ---- Blue ---- */
.callout[data-callout="right-sidebar-blue"] {
  --sidebar-bg: #f0f8ff;
  --sidebar-border: #b8d4f0;
  --sidebar-heading-bg: rgba(0, 123, 255, 0.10);
}

/* ---- Purple ---- */
.callout[data-callout="right-sidebar-purple"] {
  --sidebar-bg: #f5f0ff;
  --sidebar-border: #d4c4f0;
  --sidebar-heading-bg: rgba(111, 66, 193, 0.12);
}

/* ---- Gold ---- */
.callout[data-callout="right-sidebar-gold"] {
  --sidebar-bg: #fdf8f0;
  --sidebar-border: #f0e0b8;
  --sidebar-heading-bg: rgba(212, 160, 23, 0.12);
}

/* ---- Orange ---- */
.callout[data-callout="right-sidebar-orange"] {
  --sidebar-bg: #fff4f0;
  --sidebar-border: #f5d4b8;
  --sidebar-heading-bg: rgba(253, 126, 20, 0.12);
}

/* ---- Teal ---- */
.callout[data-callout="right-sidebar-teal"] {
  --sidebar-bg: #f0fdfa;
  --sidebar-border: #b8e8d4;
  --sidebar-heading-bg: rgba(32, 201, 151, 0.12);
}

/* ---- Pink ---- */
.callout[data-callout="right-sidebar-pink"] {
  --sidebar-bg: #fdf0f5;
  --sidebar-border: #f5c4d4;
  --sidebar-heading-bg: rgba(232, 62, 140, 0.12);
}

/* ---- Gray ---- */
.callout[data-callout="right-sidebar-gray"] {
  --sidebar-bg: #f8f9fa;
  --sidebar-border: #dee2e6;
  --sidebar-heading-bg: rgba(108, 117, 125, 0.10);
}

/* ========================================
   PART 4: MOBILE RESPONSIVE
   ======================================== */

@media screen and (max-width: 768px) {

  .callout[data-callout^="right-sidebar-"],
  .callout[data-callout="right-sidebar"] {
    float: none;
    width: 100%;
    margin: 1em 0;
    position: static;
  }
}
```

## How to use

```md
USAGE:
Add a callout to your note using one of the colors below.
Nest "sidebar-group" callouts inside it for sectioned content.

> [!right-sidebar] **Title**
> Your content here
>
> > [!sidebar-group] **Section heading**
> > [[Link one]] · [[Link two]] · [[Link three]]

COLOR OPTIONS (replace "right-sidebar" with one of these):
  right-sidebar         → default (theme-based)
  right-sidebar-red
  right-sidebar-green
  right-sidebar-blue
  right-sidebar-purple
  right-sidebar-gold
  right-sidebar-orange
  right-sidebar-teal
  right-sidebar-pink
  right-sidebar-gray
```