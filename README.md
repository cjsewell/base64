<p align="center">
  <img src="/sixty-four.png" alt="sixty-four" width="150" height="150"><br>
  Your one stop shop for base64 needs<br>
</p>

# sixty-four

![Node.js CI](https://github.com/Hexagon/sixty-four/workflows/Node.js%20CI/badge.svg?branch=master) [![npm version](https://badge.fury.io/js/sixty-four.svg)](https://badge.fury.io/js/sixty-four) [![Codacy Badge](https://app.codacy.com/project/badge/Grade/4978bdbf495941c087ecb32b120f28ff)](https://www.codacy.com/gh/Hexagon/sixty-four/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=Hexagon/sixty-four&amp;utm_campaign=Badge_Grade)
[![MIT License](https://img.shields.io/badge/license-MIT-blue.svg)](https://github.com/Hexagon/sixty-four/blob/master/LICENSE) [![jsdelivr](https://data.jsdelivr.com/v1/package/gh/hexagon/sixty-four/badge?style=rounded)](https://www.jsdelivr.com/package/gh/hexagon/sixty-four)

*   Works in Node.js >=4.0 (both require and import).
*   Works in Deno >=1.16.
*   Works in browsers as standalone, UMD or ES-module.
*   Includes [TypeScript](https://www.typescriptlang.org/) typings.

Quick examples:

```javascript
// ...
```

More [examples](#examples)...

## Installation

### Node.js

```npm install sixty-four --save```

JavaScript

```javascript
// ESM Import ...
import base64 from "sixty-four";

// ... or CommonJS Require
const base64 = require("sixty-four");
```

TypeScript

*Note that only default export is available in Node.js TypeScript, as the commonjs module is used internally.*

```typescript
import base64 from "sixty-four";

// ...
```

### Deno

JavaScript

```javascript
import base64 from "https://cdn.jsdelivr.net/gh/hexagon/sixty-four@4/src/sixty-four.js";

// ...
```

TypeScript

```typescript
import { base64 } from "https://cdn.jsdelivr.net/gh/hexagon/sixty-four@4/src/sixty-four.js";

// ...
```

### Browser 

#### Manual

*   Download latest [zipball](https://github.com/Hexagon/sixty-four/archive/refs/heads/master.zip)
*   Unpack
*   Grab ```sixty-four.min.js``` (UMD and standalone) or ```sixty-four.min.mjs``` (ES-module) from the [dist/](/dist) folder

#### CDN

To use as a [UMD](https://github.com/umdjs/umd)-module (stand alone, [RequireJS](https://requirejs.org/) etc.)

```html
<script src="https://cdn.jsdelivr.net/npm/sixty-four@1/dist/sixty-four.min.js"></script>
```

To use as a [ES-module](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Modules)

```html
<script type="module">
	import sixty-four from "https://cdn.jsdelivr.net/npm/sixty-four@/dist/sixty-four.min.mjs";

	// ... see usage section ...
</script>
```
## Documentation

Full documentation available at [hexagon.github.io/sixty-four](https://hexagon.github.io/sixty-four/sixty-four.html).

## API

The library encodes and decodes base64/base64url to and from ArrayBuffers

 - __fromArrayBuffer(buffer)__ - Encodes `ArrayBuffer` into base64 string
 - __toArrayBuffer(str)__ - Decodes base64 string to `ArrayBuffer`

 - __fromArrayBuffer(buffer, true)__ - Encodes `ArrayBuffer` into base64url string
 - __toArrayBuffer(str, true)__ - Decodes base64url string to `ArrayBuffer`

 - __fromString(str)__ - Encodes `String` into base64 string
 - __toString(str)__ - Decodes base64 string to `String`

 - __fromString(buffer, true)__ - Encodes `String` into base64url string
 - __toString(str, true)__ - Decodes base64url string to `String`

## Contributing

See [Contribution Guide](/CONTRIBUTING.md)

## License

MIT
