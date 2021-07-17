<div align="center">

![Brand Colors](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/collection)](https://www.npmjs.com/package/@brandcolors/collection)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/collection)](https://www.npmjs.com/package/@brandcolors/collection)
[![License](https://flat.badgen.net/npm/license/@brandcolors/collection)](https://www.npmjs.com/package/@brandcolors/collection)

## Introduction

Brand Colors Collection.

## Installation

```shell
npm install @brandcolors/collection
```

## Usage

### Styles

The styles will create all custom properties in CSS `root`.

<block-code>

```scss
@use "@brandcolors/collection/styles";
```

</block-code>

## Theming

```scss
@use "@brandcolors/collection" as brandcolors;

.foo {
    color: brandcolors.$twitter-primary;
    // color: #1da1f2;
    color: brandcolors.$twitter-primary-rgb;
    // color: rgb(29, 161, 242);
}
```
