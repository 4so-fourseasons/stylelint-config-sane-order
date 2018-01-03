[![npm version](https://badge.fury.io/js/%404so-fourseasons%2Fstylelint-config-sane-order.svg)](https://badge.fury.io/js/%404so-fourseasons%2Fstylelint-config-sane-order)<Paste>


# stylelint-config-sane-order

## Installation

```bash
npm i @4so-fourseasons/stylelint-config-sane-order
```

## Usage

This configuration already extends the [standard configuration](https://github.com/stylelint/stylelint-config-standard)
Just extend `stylelint-config-sane-order` inside your `stylelint.config.js`:

```js
module.exports = {
    'extends': [
        '@4so-fourseasons/stylelintconfig-sane-order'
    ],
    ...
}

```


## Enforced property order

```scss
/**
 * Multi-line comment
 */
.selector {
  // Single line comment
  // Sass extend
  @extend .svg-icon__chat--orange-peel;
  @extend .svg-icon__chat--orange-peel-dims;

  // Sass include
  @include clearfix;

  // Content for pseudo elements
  content: "";

  // Layout
  display: block;
  visibility: visible;
  float: left;
  position: absolute;
  z-index: 100;
  top: 0;
  right: 0;
  bottom: 0;
  left: 0;

  // Flex, when "display: flex;"
  flex-direction: row;
  flex-wrap: wrap;

  // Box model
  box-sizing: border-box;
  margin: 20px;
  border: 1px solid green;
  padding: 5px;
  width: 100px;
  min-width: 50px;
  max-width: 150px;
  height: 100px;
  min-height: 50px;
  max-height: 150px;

  // Visual
  background: #fff;
  color: #444;
  box-shadow: 10px 10px 5px 0 rgba(0, 0, 0, 0.75);
  opacity: 1;

  // Typography
  font: normal 1rem "MySuperAwesomeFont-Regular", sans-serif;
  text-align: center;

  // Misc in alphabetical order
  cursor: pointer;
  overflow: hidden;
  transition: all 0.3s;
  ...
}

```
