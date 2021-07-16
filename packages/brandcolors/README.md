<div align="center">

![Brand Colors](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/brandcolors)](https://www.npmjs.com/package/brandcolors)
[![Download](https://flat.badgen.net/npm/dt/brandcolors)](https://www.npmjs.com/package/brandcolors)
[![License](https://flat.badgen.net/npm/license/brandcolors)](https://www.npmjs.com/package/brandcolors)

## Introduction

Brand colors collection.

## Installation

```shell
npm install brandcolors
```

## Usage

### Styles

The styles will create all custom properties in `:root {...}`.

<block-code>

```scss
@use "@brandcolors/styles";
```

</block-code>

## Theming

```scss
@use "brandcolors";

.foo {
    color: brandcolors.$twitter-primary;
    // color: #1da1f2;
    color: brandcolors.$twitter-primary-rgb;
    // color: rgb(29, 161, 242);
}
```
