> [!NOTE]
> This repository is a fork of [NateScarlet/svg-variable-width-line](https://github.com/NateScarlet/svg-variable-width-line), adapted for use in environments without a DOM, such as Deno.

# SVG Variable width line

[![npm package](https://img.shields.io/npm/v/@hanakla/svg-variable-width-line)](https://www.npmjs.com/package/@hanakla/svg-variable-width-line)
[![GitHub Actions CI](https://github.com/hanakla/svg-variable-width-line/workflows/CI/badge.svg)](https://github.com/hanakla/svg-variable-width-line/actions)

Create svg `path` with each point can have variable width.

Can create line with `PointerEvent.pressure`.

[Demo](https://natescarlet.github.io/svg-variable-width-line/)

## Installation

```bash
npm install @hanakla/svg-variable-width-line
```

### Deno

```typescript
import * as svgVariableWidthLine from 'npm:@hanakla/svg-variable-width-line';
```

## Usage

```javascript
import * as svgVariableWidthLine from '@hanakla/svg-variable-width-line';

svgVariableWidthLine.compute({
  points: [
    { x: 0, y: 0, w: 1 },
    { x: 1, y: 0, w: 0 },
  ],
});
// { d: '<Will be path `d` data>' }
```
