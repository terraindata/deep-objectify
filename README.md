# deep-objectify
[![Build Status](https://travis-ci.org/terraindata/deep-objectify.svg?branch=master)](https://travis-ci.org/terraindata/deep-objectify)
[![version](https://img.shields.io/npm/v/deep-objectify.svg)](https://www.npmjs.org/package/deep-objectify)
[![dependencies](https://david-dm.org/terraindata/deep-objectify.svg)](https://david-dm.org/terraindata/deep-objectify)
[![devDependencies](https://david-dm.org/terraindata/deep-objectify/dev-status.svg)](https://david-dm.org/terraindata/deep-objectify#info=devDependencies)

_Curly brackets all the way down_

This is a tiny JS utility that converts deeply nested structures, which may include layers of objects and arrays, to pure nested objects.  The key feature is converting arrays to objects.  While objects and arrays are more or less equivalent in JS, it may be easier to reason about complicated data processing and storage if you can guaranteee that your complex JSON object has values that are stricly primitives or child JSON objects.

TypeScript definitions included!

## Installation

    npm install deep-objectify

## Usage

```js
var objectify = require('deep-objectify');

objectify({foo: 'bar', x: ['a', 'b']}); // -> {foo: 'bar', x: {'0': 'a', '1': 'b'}}
```

See also [deep-objectifyTests.ts](https://github.com/terraindata/deep-objectify/blob/master/deep-objectifyTests.ts).

