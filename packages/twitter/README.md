<div align="center">

![Brand Colors Twitter](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/twitter)](https://www.npmjs.com/package/@brandcolors/twitter)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/twitter)](https://www.npmjs.com/package/@brandcolors/twitter)
[![License](https://flat.badgen.net/npm/license/@brandcolors/twitter)](https://www.npmjs.com/package/@brandcolors/twitter)

## Introduction

Twitter brand colors.

## Installation

```shell
npm install @brandcolors/twitter
```

## Usage

```scss
@use "@brandcolors/twitter";

.foo {
    color: twitter.$primary;
    // color: #1da1f2;
    color: twitter.$primary-rgb;
    // color: rgb(29, 161, 242);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$primary` | Return `#...`. |
| `$primary-rgb` | Return `rgb(...)`. |
