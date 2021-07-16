<div align="center">

![Brand Colors Facebook](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/facebook)](https://www.npmjs.com/package/@brandcolors/facebook)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/facebook)](https://www.npmjs.com/package/@brandcolors/facebook)
[![License](https://flat.badgen.net/npm/license/@brandcolors/facebook)](https://www.npmjs.com/package/@brandcolors/facebook)

## Introduction

Facebook brand colors.

## Installation

```shell
npm install @brandcolors/facebook
```

## Usage

```scss
@use "@brandcolors/facebook";

.foo {
    color: facebook.$primary;
    // color: #1877f2;
    color: facebook.$primary-rgb;
    // color: rgb(24, 119, 242);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$primary` | Return `#...`. |
| `$primary-rgb` | Return `rgb(...)`. |
