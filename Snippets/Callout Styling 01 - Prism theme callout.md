↪[Collection](Collection.md)

# Callout Styling 01 - Prism theme callout

---

- author:: damiankorcz, sailKite (compiled by)
- source:: https://discord.com/channels/686053708261228577/702656734631821413/1148673835772674188

- https://github.com/damiankorcz/Prism-Theme/blob/main/src/scss/Editor/callouts.scss

---

cover:: ![](https://i.imgur.com/RaXMuJB.png)

```css
/*
MIT License

Copyright (c) 2021-2023 Damian Korcz

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

/* [Editor] Callouts */
body:not(.pt-disable-callout-styling) {
  --callout-padding: 4px;
  --callout-radius: var(--radius-m);
  --callout-background-alpha: 20%;

  .callout {
    background-color: unset;

    .callout-title {
      position: relative;
      z-index: 5;
      gap: unset;
      align-items: center;
      min-height: 36px;
      border: 2px solid;
      border-radius: var(--radius-m);
      background: rgba(var(--callout-color), 0.05);

      &:empty + .callout-content {
        padding: var(--size-4-1) var(--size-4-3);
        border-top-style: solid;
        border-top-width: 1px;
        border-radius: var(--radius-m);
      }
    }

    .callout-title-inner {
      padding: var(--size-4-1) 0;
      margin: 0 var(--size-4-1);
    }

    .callout-icon {
      align-self: unset;
      margin: 0 var(--size-4-1) 0 var(--size-4-2);
      border-radius: var(--radius-m);
    }

    .callout-fold {
      display: flex;
      align-self: unset;
      margin-top: unset;
      margin-left: auto;
    }

    .callout-content {
      padding: var(--size-4-5) var(--size-4-3) var(--size-4-1) var(--size-4-3);
      margin-top: -16px;
      border-right: 1px solid rgba(var(--callout-color));
      border-bottom: 1px solid rgba(var(--callout-color));
      border-left: 1px solid rgba(var(--callout-color));
      border-bottom-right-radius: var(--radius-m);
      border-bottom-left-radius: var(--radius-m);
      background: rgba(var(--callout-color), 0.05);
    }

    /* Type 1 */
    &[data-callout="note"] > {
      .callout-title {
        color: var(--color-grey-text);
        background-color: var(--color-grey-base);
        border-color: var(--color-grey-tint);

        .callout-icon .svg-icon {
          color: var(--color-grey-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-grey-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-grey-tint);
      }
    }

    /* Type 2 */
    &:is(
        [data-callout="abstract"],
        [data-callout="summary"],
        [data-callout="tldr"]
      )
      > {
      .callout-title {
        color: var(--color-cyan-text);
        background-color: var(--color-cyan-base);
        border-color: var(--color-cyan-tint);

        .callout-icon .svg-icon {
          color: var(--color-cyan-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-cyan-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-cyan-tint);
      }
    }

    /* Type 3 */
    &:is([data-callout="info"], [data-callout="todo"]) > {
      .callout-title {
        color: var(--color-blue-text);
        background-color: var(--color-blue-base);
        border-color: var(--color-blue-tint);

        .callout-icon .svg-icon {
          color: var(--color-blue-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-blue-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-blue-tint);
      }
    }

    /* Type 4 */
    &:is(
        [data-callout="tip"],
        [data-callout="hint"],
        [data-callout="important"]
      )
      > {
      .callout-title {
        color: var(--color-mint-text);
        background-color: var(--color-mint-base);
        border-color: var(--color-mint-tint);

        .callout-icon .svg-icon {
          color: var(--color-mint-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-mint-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-mint-tint);
      }
    }

    /* Type 5 */
    &:is(
        [data-callout="success"],
        [data-callout="check"],
        [data-callout="done"]
      )
      > {
      .callout-title {
        color: var(--color-green-text);
        background-color: var(--color-green-base);
        border-color: var(--color-green-tint);

        .callout-icon .svg-icon {
          color: var(--color-green-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-green-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-green-tint);
      }
    }

    /* Type 6 */
    &:is([data-callout="question"], [data-callout="help"], [data-callout="faq"])
      > {
      .callout-title {
        color: var(--color-yellow-text);
        background-color: var(--color-yellow-base);
        border-color: var(--color-yellow-tint);

        .callout-icon .svg-icon {
          color: var(--color-yellow-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-yellow-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-yellow-tint);
      }
    }

    /* Type 7 */
    &:is(
        [data-callout="warning"],
        [data-callout="caution"],
        [data-callout="attention"]
      )
      > {
      .callout-title {
        color: var(--color-orange-text);
        background-color: var(--color-orange-base);
        border-color: var(--color-orange-tint);

        .callout-icon .svg-icon {
          color: var(--color-orange-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-orange-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-orange-tint);
      }
    }

    /* Type 8 */
    &:is(
        [data-callout="failure"],
        [data-callout="fail"],
        [data-callout="missing"]
      )
      > {
      .callout-title {
        color: var(--color-red-text);
        background-color: var(--color-red-base);
        border-color: var(--color-red-tint);

        .callout-icon .svg-icon {
          color: var(--color-red-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-red-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-red-tint);
      }
    }

    /* Type 9 */
    &:is([data-callout="danger"], [data-callout="error"]) > {
      .callout-title {
        color: var(--color-red-text);
        background-color: var(--color-red-base);
        border-color: var(--color-red-tint);

        .callout-icon .svg-icon {
          color: var(--color-red-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-red-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-red-tint);
      }
    }

    /* Type 10 */
    &[data-callout="bug"] > {
      .callout-title {
        color: var(--color-pink-text);
        background-color: var(--color-pink-base);
        border-color: var(--color-pink-tint);

        .callout-icon .svg-icon {
          color: var(--color-pink-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-pink-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-pink-tint);
      }
    }

    /* Type 11 */
    &[data-callout="example"] > {
      .callout-title {
        color: var(--color-purple-text);
        background-color: var(--color-purple-base);
        border-color: var(--color-purple-tint);

        .callout-icon .svg-icon {
          color: var(--color-purple-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-purple-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-purple-tint);
      }
    }

    /* Type 12 */
    &:is([data-callout="quote"], [data-callout="cite"]) > {
      .callout-title {
        color: var(--color-grey-text);
        background-color: var(--color-grey-base);
        border-color: var(--color-grey-tint);

        .callout-icon .svg-icon {
          color: var(--color-grey-text);
        }
      }

      .callout-content {
        background-color: hsla(
          var(--color-grey-base-hsl),
          var(--callout-background-alpha)
        );
        border-color: var(--color-grey-tint);
      }
    }
  }
}

/* Specific styling for the unconventional use of the callout in Release Notes */
.release-notes-view .callout[data-callout] > {
  .callout-title {
    color: var(--color-grey-text);
    background-color: var(--color-grey-base);
    border-color: var(--color-grey-tint);

    .callout-icon .svg-icon {
      color: var(--color-grey-text);
    }
  }

  .callout-content {
    background-color: hsla(
      var(--color-grey-base-hsl),
      var(--callout-background-alpha)
    );
    border-color: var(--color-grey-tint);
  }
}
```
