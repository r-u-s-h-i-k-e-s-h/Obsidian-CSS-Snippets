↪[Collection](Collection.md)

# Callout styling - Sleek callout (AnuPpuccin theme)

---

- author:: Adonis, Anubis
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1040275500297375856

---

cover:: ![](https://i.imgur.com/oDUzADg.png)

```css
/*
author: Adonis, Anubis
source: https://discord.com/channels/686053708261228577/702656734631821413/1040275500297375856
support Anubis: https://www.buymeacoffee.com/anubisnekhet
*/

.callout:not(.is-collapsible) {
  padding: 0px;
}
.callout:not(.is-collapsible) .callout-content {
  padding: 0 var(--callout-title-padding) var(--callout-title-padding) var(--callout-title-padding);
}
.callout:not(.is-collapsible) .callout-title {
  background-color: rgba(var(--callout-color), 0 0.5);
  padding: var(--callout-title-padding);
  cursor: pointer;
}
.callout:not(.is-collapsible) .callout-title .callout-title-inner {
  font-weight: normal;
}

.callout:not(.is-collapsible) {
  border-color: rgba(var(--callout-color), 0.4);
  border-width: 1px;
  border-radius: var(--callout-radius);
  background-color: rgba(var(--ctp-mantle), 0.4);
}

.callout-content {
  padding: var(--callout-title-padding) var(--callout-title-padding) var(
      --callout-title-padding
    ) calc(var(--callout-title-padding) * 1.5);
  border-top: 1px dashed rgba(var(--callout-color), 0.4);
}

.callout-fold {
  padding-right: 0px;
}

.callout-title-inner {
  flex-grow: var(--anp-callout-fold-position, unset);
}

.callout {
  --callout-title-padding: var(--size-4-2);
}
.callout.is-collapsible {
  border-color: rgba(var(--callout-color), 0.4);
  border-width: 1px;
  border-radius: var(--callout-radius);
  background-color: rgba(var(--ctp-mantle), 0.4);
  --bold-weight: bolder;
}
.callout.is-collapsible .callout-fold {
  padding-right: 0px;
}
.callout.is-collapsible .callout-title-inner {
  flex-grow: var(--anp-callout-fold-position, unset);
}
.callout.is-collapsible.is-collapsed {
  padding: 0;
}
.callout.is-collapsible.is-collapsed .callout-title {
  background-color: rgba(var(--callout-color), 0.1);
  padding: var(--callout-title-padding);
  cursor: pointer;
}
.callout.is-collapsible.is-collapsed .callout-content {
  display: none;
}
.callout.is-collapsible:not(.is-collapsed) {
  padding: 0px 0px var(--callout-title-padding) 0px;
}
.callout.is-collapsible:not(.is-collapsed) .callout-title {
  background-color: rgba(var(--callout-color), 0.1);
  padding: var(--callout-title-padding);
  border-color: rgba(var(--callout-color), 0.4);
  cursor: pointer;
}
.callout.is-collapsible:not(.is-collapsed) .callout-content {
  padding: var(--callout-title-padding) var(--callout-title-padding) 0 calc(var(
          --callout-title-padding
        ) * 1.5);
  border-top: 1px dashed rgba(var(--callout-color), 0.4);
}
.callout:not(.is-collapsible) {
  padding: 0px;
}
.callout:not(.is-collapsible) .callout-title {
  background-color: rgba(var(--callout-color), 0.1);
  padding: var(--callout-title-padding);
  border-color: rgba(var(--callout-color), 0.4);
}
.callout .list-collapse-indicator {
  margin-left: -35px;
  padding-right: 3px;
}

/*# sourceMappingURL=anuppuccin-sleek-callout.css.map */
```
