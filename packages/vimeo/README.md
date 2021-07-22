<div align="center">

![Brand Colors Vimeo](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/vimeo)](https://www.npmjs.com/package/@brandcolors/vimeo)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/vimeo)](https://www.npmjs.com/package/@brandcolors/vimeo)
[![License](https://flat.badgen.net/npm/license/@brandcolors/vimeo)](https://www.npmjs.com/package/@brandcolors/vimeo)

## Introduction

Vimeo Brand Colors.

## Installation

```shell
npm install @brandcolors/vimeo
```

## Usage

### Styles

<block-code>

```scss
@use "@brandcolors/vimeo/styles";
```

</block-code>

The styles will create all custom properties in CSS `root`. If you want this custom properties anywhere else, use the
public mixin `custom-properties`.

## Theming

```scss
@use "@brandcolors/vimeo";

.foo {
    color: vimeo.$primary;
    // color: #1ab7ea;
    color: vimeo.$primary-rgb;
    // color: rgb(26, 183, 234);
}
```

### Custom Properties

```scss
@use "@brandcolors/vimeo";

:root {
    @include vimeo.custom-properties(primary);
    // --bc-vimeo-primary: #1ab7ea;
    @include vimeo.custom-properties(primary-rgb);
    // --bc-vimeo-primary-rgb: rgb(26, 183, 234);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$blue` | Return blue hex value. |
| `$dark-forest` | Return dark forest hex value. |
| `$primary` | Return primary _(a.k.a blue)_ hex value. |
| `$primary-rgb` | Return primary RGB value. |

### Mixins

| Mixin | Description |
| --- | --- |
| `custom-properties($values...)` | Create dedicated custom property. If the `$values` is empty, the mixin will create all styles by default. |
