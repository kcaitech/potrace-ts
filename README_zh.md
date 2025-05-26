# @kcaitech/potrace-ts

TypeScript 实现的 Potrace 库，用于将位图转换为可缩放矢量图形（SVG）。

> Fork 自 [node-potrace](https://github.com/iwsfg/node-potrace.git)

## 简介

Potrace 是一个用于将位图（如 PNG、JPEG 等）转换为矢量图形的工具。这个库是其 TypeScript 实现版本，提供了更好的类型支持。

## 安装

```bash
# 使用 npm
npm install @kcaitech/potrace-ts

```

## 使用示例

```typescript
import { Potrace } from "@kcaitech/potrace-ts";
...
// 图片转svg path
const imgdata: ImageData = canvas.getImageData(0, 0, size, size)
const potrace = new Potrace(imgdata, () => {})
const path = potrace.getSVGPath({ x: 1, y: 1 }, { x: 0, y: 0 });
```

## 开发

```bash
# 安装依赖
npm i

# 构建
npm run build

```

## 许可证

本项目基于 GPLv2 许可证，继承自[node-potrace](https://github.com/iwsfg/node-potrace.git)，详情请查看 [LICENSE.txt](./LICENSE.txt) 文件。

