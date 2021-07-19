<div align="center">

![Brand Colors LinkedIn](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/linkedin)](https://www.npmjs.com/package/@brandcolors/linkedin)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/linkedin)](https://www.npmjs.com/package/@brandcolors/linkedin)
[![License](https://flat.badgen.net/npm/license/@brandcolors/linkedin)](https://www.npmjs.com/package/@brandcolors/linkedin)

## Introduction

LinkedIn Brand Colors.

## Installation

```shell
npm install @brandcolors/linkedin
```

## Usage

### Styles

<block-code>

```scss
@use "@brandcolors/linkedin/styles";
```

</block-code>

The styles will create all custom properties in CSS `root`. If you want this custom properties anywhere else, use the
public mixin `custom-properties`.

## Theming

```scss
@use "@brandcolors/linkedin";

.foo {
    color: linkedin.$primary;
    // color: #1da1f2;
    color: linkedin.$primary-rgb;
    // color: rgb(29, 161, 242);
}
```

### Custom Properties

```scss
@use "@brandcolors/linkedin";

:root {
    @include linkedin.custom-properties(primary);
    // --bc-linkedin-primary: #1da1f2;
    @include linkedin.custom-properties(primary-rgb);
    // --bc-linkedin-primary-rgb: rgb(29, 161, 242);
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
