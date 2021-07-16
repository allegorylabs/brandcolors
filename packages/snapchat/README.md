<div align="center">

![Brand Colors Snapchat](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/snapchat)](https://www.npmjs.com/package/@brandcolors/snapchat)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/snapchat)](https://www.npmjs.com/package/@brandcolors/snapchat)
[![License](https://flat.badgen.net/npm/license/@brandcolors/snapchat)](https://www.npmjs.com/package/@brandcolors/snapchat)

## Introduction

Snapchat brand colors.

## Installation

```shell
npm install @brandcolors/snapchat
```

## Usage

```scss
@use "@brandcolors/snapchat";

.foo {
    color: snapchat.$primary;
    // color: #fffc00;
    color: snapchat.$primary-rgb;
    // color: rgb(255, 252, 0);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$primary` | Return `#...`. |
| `$primary-rgb` | Return `rgb(...)`. |
