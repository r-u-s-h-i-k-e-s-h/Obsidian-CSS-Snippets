---
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1168178314318458980
cover: "[[img-calendar - rainbow headers.webp]]"
obsidian-version: 1.12.7
installer-version: 1.12.7
dependencies: calendar
---
# calendar - rainbow headers

![](../attachments/img-calendar%20-%20rainbow%20headers.webp)

## Snippet

```css
/*
author: sailKite
source: https://discord.com/channels/686053708261228577/702656734631821413/1168178314318458980
modified original code for light and dark theme
*/

.theme-light .container#calendar-container .calendar {
  &>thead>tr:first-of-type {
    &>th:nth-child(1) {
      color: #d90429;
    }

    &>th:nth-child(2) {
      color: #f26419;
    }

    &>th:nth-child(3) {
      color: #a37a00;
    }

    &>th:nth-child(4) {
      color: #007200;
    }

    &>th:nth-child(5) {
      color: #0056b3;
    }

    &>th:nth-child(6) {
      color: #4b0082;
    }

    &>th:nth-child(7) {
      color: #7209b7;
    }
  }
}

.theme-dark .container#calendar-container .calendar {
  &>thead>tr:first-of-type {
    &>th:nth-child(1) {
      color: #ff4d6d;
    }

    &>th:nth-child(2) {
      color: #ff8c32;
    }

    &>th:nth-child(3) {
      color: #ffd60a;
    }

    &>th:nth-child(4) {
      color: #39ff14;
    }

    &>th:nth-child(5) {
      color: #38b000;
    }

    &>th:nth-child(6) {
      color: #9d4edd;
    }

    &>th:nth-child(7) {
      color: #ff70a6;
    }
  }
}

#calendar-container .calendar .today {
  font-weight: 700;
}
```
