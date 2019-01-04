# @gera2ld/rem

![NPM](https://img.shields.io/npm/v/@gera2ld/rem.svg)
![License](https://img.shields.io/npm/l/@gera2ld/rem.svg)
![Downloads](https://img.shields.io/npm/dt/@gera2ld/rem.svg)

Adapt to different screens using rem.

## Installation

```sh
$ yarn add @gera2ld/rem
```

## Usage

```js
import { scaleWidth } from '@gera2ld/rem';

scaleWidth();
// or
scaleWidth({
  mode: 'px',
  resize: false,
});
```

### Options

- `mode`

  - `'vw'`

    Use `vw` as root unit if supported.

  - `'px'`

    Use `px` as root unit.

  By default, if `vw` is supported, `mode` is set to `'vw'`, otherwise `'px'`.

- `resize`

  Whether the font size of root should be updated on resize. By default, `resize` is set to `true` if `vw` is not supported, otherwise `false`.
