# deepObjectify
[![Build Status](https://travis-ci.org/terraindata/deepObjectify.svg?branch=master)](https://travis-ci.org/terraindata/deepObjectify)
[![version](https://img.shields.io/npm/v/deepObjectify.svg)](https://www.npmjs.org/package/deepObjectify)
[![dependencies](https://david-dm.org/terraindata/deepObjectify.svg)](https://david-dm.org/terraindata/deepObjectify)
[![devDependencies](https://david-dm.org/terraindata/deepObjectify/dev-status.svg)](https://david-dm.org/terraindata/deepObjectify#info=devDependencies)

_Curly brackets all the way down_

This is a tiny JS utility that converts deeply nested structures, which may include layers of objects and arrays, to pure nested objects.  The key feature is converting arrays to objects.  While objects and arrays are more or less equivalent in JS, it may be easier to reason about complicated data processing and storage if you can guaranteee that your complex JSON object has values that are stricly primitives or child JSON objects.

TypeScript definitions included!

## Installation

    npm install deepObjectify

## Usage

```js
var objectify = require('deepObjectify');

objectify({foo: 'bar', x: ['a', 'b']}); // -> {foo: 'bar', x: {'0': 'a', '1': 'b'}}
```

See also [deepObjectifyTests.ts](https://github.com/terraindata/deepObjectify/blob/master/deepObjectifyTests.ts).

