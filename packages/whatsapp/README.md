<div align="center">

![Brand Colors WhatsApp](.github/logo.svg)

</div>

[![Version](https://flat.badgen.net/npm/v/@brandcolors/whatsapp)](https://www.npmjs.com/package/@brandcolors/whatsapp)
[![Download](https://flat.badgen.net/npm/dt/@brandcolors/whatsapp)](https://www.npmjs.com/package/@brandcolors/whatsapp)
[![License](https://flat.badgen.net/npm/license/@brandcolors/whatsapp)](https://www.npmjs.com/package/@brandcolors/whatsapp)

## Introduction

WhatsApp Brand Colors.

## Installation

```shell
npm install @brandcolors/whatsapp
```

## Usage

### Styles

The styles will create custom properties in CSS `root`. If you want this custom properties anywhere else, use the public
mixin `custom-properties`.

<block-code>

```scss
@use "@brandcolors/whatsapp/styles";
```

</block-code>

## Theming

```scss
@use "@brandcolors/whatsapp";

.foo {
    color: whatsapp.$primary;
    // color: #1da1f2;
    color: whatsapp.$primary-rgb;
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
| `custom-properties` | Create custom property for each variables register. Ex. `--bc-whatsapp-primary: #1da1f2` |
