<div align="center">

![Brand Colors Facebook](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/facebook)](https://www.npmjs.com/package/@brandcolors/facebook)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/facebook)](https://www.npmjs.com/package/@brandcolors/facebook)
[![License](https://flat.badgen.net/npm/license/@brandcolors/facebook)](https://www.npmjs.com/package/@brandcolors/facebook)

## Introduction

Facebook Brand Colors.

## Installation

```shell
npm install @brandcolors/facebook
```

## Usage

### Styles

<block-code>

```scss
@use "@brandcolors/facebook/styles";
```

</block-code>

The styles will create all custom properties in CSS `root`. If you want this custom properties anywhere else, use the
public mixin `custom-properties`.

## Theming

```scss
@use "@brandcolors/facebook";

.foo {
    color: facebook.$primary;
    // color: #1877f2;
    color: facebook.$primary-rgb;
    // color: rgb(24, 119, 242);
}
```

### Custom Properties

```scss
@use "@brandcolors/facebook";

:root {
    @include facebook.custom-properties(primary);
    // --bc-facebook-primary: #1877f2;
    @include facebook.custom-properties(primary-rgb);
    // --bc-facebook-primary-rgb: rgb(24, 119, 242);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$primary` | Return `#...` color. |
| `$primary-rgb` | Return `rgb(...)` color. |

### Mixins

| Mixin | Description |
| --- | --- |
| `custom-properties($values...)` | Create dedicated custom property. If the `$values` is empty, the mixin will create all styles by default. |
