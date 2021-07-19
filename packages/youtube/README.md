<div align="center">

![Brand Colors YouTube](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/youtube)](https://www.npmjs.com/package/@brandcolors/youtube)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/youtube)](https://www.npmjs.com/package/@brandcolors/youtube)
[![License](https://flat.badgen.net/npm/license/@brandcolors/youtube)](https://www.npmjs.com/package/@brandcolors/youtube)

## Introduction

YouTube Brand Colors.

## Installation

```shell
npm install @brandcolors/youtube
```

## Usage

### Styles

<block-code>

```scss
@use "@brandcolors/youtube/styles";
```

</block-code>

The styles will create all custom properties in CSS `root`. If you want this custom properties anywhere else, use the
public mixin `custom-properties`.

## Theming

```scss
@use "@brandcolors/youtube";

.foo {
    color: youtube.$primary;
    // color: #FF0000;
    color: youtube.$primary-rgb;
    // color: rgb(255, 0, 0);
}
```

### Custom Properties

```scss
@use "@brandcolors/youtube";

:root {
    @include youtube.custom-properties(primary);
    // --bc-youtube-primary: #FF0000;
    @include youtube.custom-properties(primary-rgb);
    // --bc-youtube-primary-rgb: rgb(255, 0, 0);
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
| `custom-properties($values...)` | Create dedicated custom property. If the `$values` is empty, the mixin will create all styles by default. |
