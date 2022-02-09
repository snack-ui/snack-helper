# Snack-helper

[![npm](https://img.shields.io/npm/v/snack-helper.svg)](https://www.npmjs.com/package/snack-helper)
[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/nzbin/snack-helper)
[![Gitter](https://img.shields.io/gitter/room/snack-helper/snack-helper.svg)](https://gitter.im/snack-ui/snack-helper)

Snack-helper is a universal CSS helper library.

## Installation

```bash
$ npm install snack-helper --save
```

## Usage

```scss
@use 'snack-helper';
```

The @use-based Sass API is only available in the version 2.2.0 or above.

## Customization

Some helpers can be customized with variables. Take the spacing for example.

Here is the default spacing variable.

```scss
$spacer: 1rem !default;
$spacers: (
  0: 0,
  4: $spacer * .25,
  8: $spacer * .5,
  12: $spacer * .75,
  16: $spacer,
  24: $spacer * 1.5,
  32: $spacer * 2,
  48: $spacer * 3
) !default;
```

You can cover the whole original spacing with `$spacers` as you like.

```scss
@use 'snack-helper' with (
  $spacers: (
    0: 0,
    1: .25rem,
    2: .5rem,
    3: .75rem,
    4: 1rem,
    5: 1.5rem
  )
);
```

If you just want to extend the original spacing, you can use the `$spacers-extend`;

```scss
@use '~snack-helper' with (
  $spacers-extend: (
    5: 5px,
    10: 10px,
    15: 15px
  )
);
```

## Overview

- [Color](https://snack-ui.github.io/snack-helper/#colors)
- [Spacing](https://snack-ui.github.io/snack-helper/#spacing)
- [Sizing](https://snack-ui.github.io/snack-helper/#size)
- [Border](https://snack-ui.github.io/snack-helper/#borders)
- [Rounded](https://snack-ui.github.io/snack-helper/#rounded)
- [Shadow](https://snack-ui.github.io/snack-helper/#shadows)
- [Text](https://snack-ui.github.io/snack-helper/#text)
- [Alignment](https://snack-ui.github.io/snack-helper/#alignment)
- [Display](https://snack-ui.github.io/snack-helper/#display)
- [Position](https://snack-ui.github.io/snack-helper/#position)
- [Flexbox](https://snack-ui.github.io/snack-helper/#flexbox)

## License

MIT License
