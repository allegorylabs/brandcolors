<div align="center">

![Brand Colors LinkedIn](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/linkedin)](https://www.npmjs.com/package/@brandcolors/linkedin)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/linkedin)](https://www.npmjs.com/package/@brandcolors/linkedin)
[![License](https://flat.badgen.net/npm/license/@brandcolors/linkedin)](https://www.npmjs.com/package/@brandcolors/linkedin)

## Introduction

LinkedIn brand colors.

## Installation

```shell
npm install @brandcolors/linkedin
```

## Usage

### Styles

The styles will create custom properties in `:root {...}`. If you want this custom properties anywhere else, use the
public mixin `custom-properties`.

<block-code>

```scss
@use "@brandcolors/linkedin/styles";
```

</block-code>

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

## API

### Variables

| Variable | Value |
| --- | --- |
| `$primary` | Return `#...`. |
| `$primary-rgb` | Return `rgb(...)`. |

### Mixins

| Mixin | Description |
| --- | --- |
| `custom-properties` | Create custom property for each variables register. Ex. `--bc-linkedin-primary: #1da1f2` |
