# @kcaitech/potrace-ts

A TypeScript implementation of Potrace library for converting bitmaps to scalable vector graphics (SVG).

> Forked from [node-potrace](https://github.com/iwsfg/node-potrace.git)

## Introduction

Potrace is a tool for converting bitmap images (such as PNG, JPEG, etc.) into vector graphics. This library is its TypeScript implementation version, providing better type support.

## Installation

```bash
# Using npm
npm install @kcaitech/potrace-ts

```

## Usage Example

```typescript
import { Potrace } from "@kcaitech/potrace-ts";
...
// Convert image to SVG path
const imgdata: ImageData = canvas.getImageData(0, 0, size, size)
const potrace = new Potrace(imgdata, () => {})
const path = potrace.getSVGPath({ x: 1, y: 1 }, { x: 0, y: 0 });
```

## Development

```bash
# Install dependencies
npm i

# Build
npm run build

```

## License

This project is licensed under GPLv2, inherited from [node-potrace](https://github.com/iwsfg/node-potrace.git). For more details, please check the [LICENSE.txt](./LICENSE.txt) file.

