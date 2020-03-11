# @tonaljs/chord-detect ![tonal](https://img.shields.io/badge/@tonaljs-chord-detect-yellow.svg?style=flat-square) [![npm version](https://img.shields.io/npm/v/@tonaljs/chord-detect.svg?style=flat-square)](https://www.npmjs.com/package/@tonaljs/chord-detect)

## Usage

With ES6 `import`:

```js
import { Chord } from "@tonaljs/tonal";
```

With ES5 `require`:

```js
const { Chord } = require("@tonaljs/tonal");
```

Standalone:

```js
import { detect } from "@tonaljs/chord-detect";
```

## API

### `Chord.detect(notes: string[]) => string[]`

Examples:

```js
Chord.detect(["D", "F#", "A", "C"]); // => ["D7"]
Chord.detect(["F#", "A", "C", "D"]); // => ["D7/F#"]
Chord.detect(["A", "C", "D", "F#"]); // => ["D7/A"]
Chord.detect(["E", "G#", "B", "C#"]); // => ["E6", "C#m7/E"]
```