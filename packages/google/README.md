<div align="center">

![Brand Colors Google](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/google)](https://www.npmjs.com/package/@brandcolors/google)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/google)](https://www.npmjs.com/package/@brandcolors/google)
[![License](https://flat.badgen.net/npm/license/@brandcolors/google)](https://www.npmjs.com/package/@brandcolors/google)

## Introduction

Google Brand Colors.

## Installation

```shell
npm install @brandcolors/google
```

## Usage

### Styles

<block-code>

```scss
@use "@brandcolors/google/styles";
```

</block-code>

The styles will create all custom properties in CSS `root`. If you want this custom properties anywhere else, use the
public mixin `custom-properties`.

## Theming

```scss
@use "@brandcolors/google";

.foo {
    color: google.$primary;
    // color: #4285f4;
    color: google.$primary-rgb;
    // color: rgb(66, 133, 244);
}
```

### Custom Properties

```scss
@use "@brandcolors/google";

:root {
    @include google.custom-properties(primary);
    // --bc-google-primary: #4285f4;
    @include google.custom-properties(primary-rgb);
    // --bc-google-primary-rgb: rgb(66, 133, 244);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$primary` | Return hex value color. |
| `$primary-rgb` | Return `rgb` color. |
| `$blue` | Return hex value color. |
| `$green` | Return hex value color. |
| `$yellow` | Return hex value color. |
| `$red` | Return hex value color. |

### Mixins

| Mixin | Description |
| --- | --- |
| `custom-properties($values...)` | Create dedicated custom property. If the `$values` is empty, the mixin will create all styles by default. |
