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

```scss
@use "@brandcolors/linkedin";

.foo {
    color: linkedin.$brand;
    // color: #1da1f2;
    color: linkedin.$brand-rgb;
    // color: rgb(29, 161, 242);
}
```

## API

### Variables

| Variable | Value |
| --- | --- |
| `$brand` | Return `#...`. |
| `$brand-rgb` | Return `rgb(...)`. |
