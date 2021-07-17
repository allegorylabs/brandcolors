<div align="center">

![Brand Colors Snapchat](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/snapchat)](https://www.npmjs.com/package/@brandcolors/snapchat)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/snapchat)](https://www.npmjs.com/package/@brandcolors/snapchat)
[![License](https://flat.badgen.net/npm/license/@brandcolors/snapchat)](https://www.npmjs.com/package/@brandcolors/snapchat)

## Introduction

Snapchat Brand Colors.

## Installation

```shell
npm install @brandcolors/snapchat
```

## Usage

### Styles

The styles will create custom properties in CSS `root`. If you want this custom properties anywhere else, use the public
mixin `custom-properties`.

<block-code>

```scss
@use "@brandcolors/snapchat/styles";
```

</block-code>

## Theming

```scss
@use "@brandcolors/snapchat";

.foo {
    color: snapchat.$primary;
    // color: #fffc00;
    color: snapchat.$primary-rgb;
    // color: rgb(255, 252, 0);
}
```

### Custom Properties

```scss
@use "@brandcolors/snapchat";

:root {
    @include snapchat.custom-properties(primary);
    // --bc-snapchat-primary: #fffc00;
    @include snapchat.custom-properties(primary-rgb);
    // --bc-snapchat-primary-rgb: rgb(255, 252, 0);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$primary` | Return `#...`. |
| `$primary-rgb` | Return `rgb(...)`. |

### Mixins

| Mixin | Description |
| --- | --- |
| `custom-properties($values...)` | Create custom property on `root`. If the `$values` is empty, the mixin will create all styles by default. |
