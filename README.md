![Kablam Logo](kablam.png)

[**Kablam.js**](https://kablamjs.com/) is a fork of [Kaboom.js](https://kaboomjs.com/)

This fork has some principles which really differentiate it from the main Kaboom library:
- Improved Pysics Engine:
    - The physics/collisions are a bit dodgy on Kaboom, which is the main reason I made this fork.
- No NFT Stuff:
    - They aren't good for the environment, I don't like them, on top of the fact that their use is limited, at most.
- Separated assets, lubrarym and everything else:
    - In kaboom, the library, website, demos, and assets are all in one massive repository. If it isn't obvious, this is a bit of an issue in terms of performance, as downloading a whole megabyte to a machine to run a simple game is very :|.
- Better FPS:
    - This is on the backburner right now, but general performance improvements are to come, I just need to figure out in what areas these will occur. 
- Greater Control:
    - This library gives you greater control over the elements at hand. No more creating something and theres no way to get resulting element. For example, you'll actually be able to get the audio context from a played audio file.

## Examples

> I've removed the examples section from the readme of this fork, mainly as I feel it will become neglected, along with the fact that any Kaboom.js code should work A-OK.

## Usage

### NPM

```sh
$ npm install kablam
```

```js
import kaboom from "kablam";

kaboom();

add([
    text("oh hi"),
    pos(80, 40),
]);
```

also works with CommonJS

```js
const kaboom = require("kablam");
```

Note that you'll need to use a bundler like `esbuild` or `webpack` to use Kaboom with NPM

### Browser CDN

This exports a global `kaboom` function

```html
<script src="https://unpkg.com/kablam/dist/kablam.js"></script>
<script>
kaboom();
</script>
```

or use with es modules

```html
<script type="module">
import kaboom from "https://unpkg.com/kablam/dist/kablam.mjs";
kaboom();
</script>
```

works all CDNs that supports NPM packages, e.g. jsdelivr, skypack

## Dev

1. `npm run setup` to setup first time (installing dev packages)
1. `npm run dev` to watch & build lib and the website (the website might take some time to build for the first time)
1. go to http://localhost:3000/play
1. edit demos in `demo/` to test
1. make sure not to break any existing demos

also check out [CONTRIBUTION.md](CONTRIBUTING.md)

## Community

[Github Discussions](https://github.com/pieromqwerty/kablam/discussions)

### Misc

- Thanks to [abrudz](https://github.com/abrudz) for the amazing [APL386 font](https://abrudz.github.io/APL386/)
- Thanks to [Polyducks](http://polyducks.co.uk/) for the amazing [kitchen sink font](https://polyducks.itch.io/kitchen-sink-textmode-font) font
- Thanks to [0x72](https://0x72.itch.io/) for the amazing [Dungeon Tileset](https://0x72.itch.io/dungeontileset-ii)
- Thanks to [Kenney](https://kenney.nl/) for the amazing [1-Bit Platformer Pack](https://kenney.nl/assets/bit-platformer-pack)
- Find bitmap fonts: [Oldschool PC Font](https://int10h.org/oldschool-pc-fonts)
- Featured on [Console 50](https://console.substack.com/p/console-50)
- Thanks to [Umayr](https://github.com/umayr) for kindly offering the "kaboom" npm package name
- Please buy fireworks on [kaboom.com](http://www.kaboom.com/)
- Documentation for v0.5 [here](https://kaboomlegacy.repl.co/)
- [How to do a KABOOM on a Trampoline](https://www.youtube.com/watch?v=3CemcWdc_Hc)
