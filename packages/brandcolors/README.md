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

```scss
@use "brandcolors";

.foo {
    color: brandcolors.$twitter-brand;
    // color: #1da1f2;
    color: brandcolors.$twitter-brand-rgb;
    // color: rgb(29, 161, 242);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$brand` | Return `#...`. |
| `$brand-rgb` | Return `rgb(...)`. |
