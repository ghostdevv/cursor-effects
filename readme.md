# 90's Cursor Effects
_"Knowing the codes" used to be all the rage, I want to bring a few back._

A repo of the old effects that inspired creativity and the desire to learn at least a little code around the world. Modernised so they're a little more efficient, and just as annoying (and twice as fun) as they were before. [Have a play here](https://tholman.com/cursor-effects).

The current effects are:
- Emoji Rain
- Elastic Emoji
- Ghost Following
- Following Dot
- Bubbles Particles
- Snowflake Particles
- Fairy Dust

# How to Use

You need to include the following script tag in your webpage (see next section if you want to use this package via npm).

```html
<script src="https://cdn.jsdelivr.net/npm/cursor-effects/dist/browser.js"></script>
```

Alternatively you can use a `type="module"` script on newer browsers with a import statement

```html
<script type="module">
import cursoreffects from 'https://cdn.jsdelivr.net/npm/cursor-effects@2/dist/esm.js';

new cursoreffects.ghostCursor();
</script>
```

And then create a new instance of its type in your JavaScript. The script will create the canvas that is used, so nothing else is really needed.

```js
new cursoreffects.ghostCursor();
```

You can also target specific elements, to have the canvas appear inside those, for example:

```js
const targetElement = document.querySelector("#ghost")
new cursoreffects.ghostCursor({element: targetElement});
```

## Specific Customization

A few of these have custom options as well (if you are interested in more options, opening an issue or PR is the way to go).

### springyEmojiCursor

You can change the emoji in `springyEmojiCursor`'s emoji with the `emoji` a single string emoji.

```js
new cursoreffects.springyEmojiCursor({emoji: "🤷‍♂️"});
```

### fairyDustCursor

You can change the emoji in `fairyDustCursor`'s colors with the `colors` option (an array of colors)

```js
new cursoreffects.fairyDustCursor({colors: ["#ff0000", "#00ff00", "#0000ff"]});
```

### emojiCursor


You can change the emoji in `emojiCursor`'s emoji with the `emoji` option (a list of emoji)

```js
new cursoreffects.emojiCursor({emoji: ["🔥", "🐬", "🦆"]});
```

# NPM

```sh
npm install cursor-effects
```

```js
import { emojiCursor } from 'cursor-effects';

new emojiCursor({ emoji: ["🔥", "🐬", "🦆"] });
```

# License

MIT af, but if you're using the scripts a [GitHub sponsorship](https://github.com/sponsors/tholman) or [shouting me a coffee](https://www.buymeacoffee.com/tholman) would always be appreciated :)
