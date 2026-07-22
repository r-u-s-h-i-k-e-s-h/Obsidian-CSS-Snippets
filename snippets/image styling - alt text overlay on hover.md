---
author:
  - sailKite
source: https://discord.com/channels/686053708261228577/694233507500916796/1169731141813674075
cover: "[[gif-image styling - alt text overlay on hover.gif]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
---
# Image styling - alt text overlay on hover

![](../attachments/gif-image%20styling%20-%20alt%20text%20overlay%20on%20hover.gif)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/694233507500916796/1169731141813674075
*/

.internal-embed.image-embed {
  position: relative;

  &:hover::after {
    content: attr(alt);
    display: block;
    position: absolute;
    background-color: var(--background-primary);
    border: 1px solid var(--color-base-30);
    border-radius: var(--size-2-2);
    padding: 0.5em;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
  }
}
```

## Usage

```md
![[image 01.jpg|Ut enim ad minim veniam]]
```
