↪[Collection](Collection.md)

# Tag styling - Hide hash symbol

---

- author:: Bluemoondragon07, FireIsGood
- source:: https://forum.obsidian.md/t/hiding-hashtags-but-again/61706?u

---

cover:: ![](https://i.imgur.com/wqMrZpi.png)

```css
/*
author: Bluemoondragon07, FireIsGood
source: https://forum.obsidian.md/t/hiding-hashtags-but-again/61706?u
*/

@font-face {
  font-family: "Formular";
  src: url("data:font/woff;charset=utf-8;base64,d09GRgABAAAAAAXMAA4AAAAACOAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAAABHREVGAAAFZAAAABYAAAAWABMABkdQT1MAAAV8AAAAIAAAACBEdkx1R1NVQgAABZwAAAAvAAAAMCN+JIxPUy8yAAACDAAAAEcAAABgII84HWNtYXAAAAJUAAAAMQAAADwAOwB9Z2FzcAAABVwAAAAIAAAACP//AANnbHlmAAABRAAAACgAAAAoKX11F2hlYWQAAAGcAAAANgAAADYW4dEnaGhlYQAAAewAAAAgAAAAJA/2Cc9obXR4AAAB1AAAABgAAAAYDeYAd2xvY2EAAAGMAAAADQAAAA4APAA8bWF4cAAAAWwAAAAeAAAAIABLAEVuYW1lAAACiAAAAq4AAAXocAf8uHBvc3QAAAU4AAAAJAAAADNVXVC5AAIAdwAAA8MFtgADAAcAADMRIRElIREhdwNM/T8CNf3LBbb6SoEEtHjaY2BkYGBgY3BiYGYAASYgZmQAiTmA+QwACZIAkQAAeNpjYGAQQUAAAt4AeQAAAAABAAAAAgCDDlp/b18PPPUACwgAAAAAAM8sf4QAAAAA4KMGkP+m/lgITAc7AAAACAACAAAAAAAABDkAdwAAAAACqgAAAAAAAAI5AAAEygAAeNpjYGRgYLP8Z8l4krv//zIGBg4fBqAICmADAH24BNx42mNgZrnJOIGBlYGB1ZjlLAMDwywIzXSWIY0pC0gzIAFGBnTgwKDAoMxm+c+S8ST7XcY3CgwM08EKfzCdAlIKDEwAU4UM+QB42mNgYGBiYGBgBmIRIMkIplkYNIA0G5BmBMoqMCj//w/kg+n/T/4/AqsCAgCI4wiyAAAAeNqtUrtu1EAUvfZu3g/RISGERqJJpMReVkFityKJlBSRUEgRiXJsjx+s12ONZ9dxw5/QUFJS8QF8AZ9CS8Px7CRrIJEosOWZc1/nnrkeInrmFOTQ4nmHb4EdWoe1wC6tEbe4Ry8ptbjfyVmhHfpo8WrHv0Zv6bPF67RHPy3e6ODNTt8teuw8t3i7g3dozxlbvEtPnQBKnP4GrC/OB4sdeuQOLHZp131tcY/eu28s7ndyVuiJ+9Xi1Y5/jT653y1ep8uetnijgzc7fbfI632zeLuDd5D/w+JdetU/OZVlo7Ik1Wwv3GfDwYujQywjFjTsnDe8EOyEJxGvuIJxwK4bHqaiyvmcXWQqy0UxkR47znNmSCqmRCXUXETemVTTWc7VlUjabUHW5VpS3TGN2W3VuJUyuhaqymTBht5gMLzMBa8EGsRCMS2ZTgVbqq9EqNvUWCoTiWWhmVY8ElOuJoxrrbJgZlIKqbNQVN6/ni/Vuhz7fl3XXqBkXcTyxpMqOS4aNoOgOtOpnGlWCjXNKqM3q1ipZJoFmRaRLe+W+jkEFKHw6ZQkldSQoowS3GJNDLcwpH3sQxrQCzqiQ4tG8AXIZXSOu9/gK0jAOgFKKMJa4VM2coDItcEheAViOfAc3gv0avvl8BY0gQIP3mPYOfalkspYbaXAPscaIfMM+YqmNDN8iq7gT+6srrKHdN2n6m9NY3T/s9f4biojsLSqKtRIVLR+D5EB9kvDwo3uxQlik8twJmnW1ETum31bEwLdssZGwbImNn5tPAo9IninRtsEPg6vNnwBNC9ZCuytFZoTe//9/6Wmb4n5+Hhr83rQoBCrkdOqvoGnPUuCP12YWzSzE6rB1Z5PGs0MPMJMPUN8Od/M3IfScKbmhG1Veyd+7/5QVx96FxMozOr/AnWqLjEAAHjaY2BiAIP/DAxpDNgAGxAzMjAxMjEwM7Cx+IX6+AAAP3gCvAAAAAH//wACAAEAAAAMAAAAAAAAAAIAAQADAAUAAQAAAAEAAAAKABwAHgABREZMVAAIAAQAAAAA//8AAAAAAAB42mNgZGBg4GLQYdBjYHZx8wlhEEmuLMphkMtJLMljkGNgAcoy/P/PAAcArlkHTgA=")
    format("woff");
}

/* Hide hashtag (reading mode) */
a.tag {
  font-family: "Formular", var(--font-text);
  padding: 9px 0.55em 5px 0;
}
a.tag:hover {
  padding: 5px 7px 5px 7px !important;
  font-family: var(--font-text);
}

/* Hide hashtag (live preview mode) */
.cm-line:not(.cm-active) .cm-hashtag-begin {
  display: none;
}
.cm-line:not(.cm-active) .cm-hashtag-end {
  border-radius: var(--tag-radius) !important;
  padding-left: var(--tag-padding-x);
  border-left: var(--tag-border-width) solid var(--tag-border-color);
}

/* prevent overlapping tags on separate lines */
p:has(.tag ~ br ~ .tag) {
  line-height: 2;
}
.cm-line:has(.cm-meta):has(+ .cm-line .cm-meta) {
  padding-bottom: 6px;
}
```
