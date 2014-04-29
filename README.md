LZW
-------------

This is LZW compression algorithm 

## Install

```bash
npm install node-lzw
```

## Example

```app.js
"use strict";

var lzw = require("node-lzw");
var buffer = "qwertyuiopasdfghjklzxcvbnm1234567890";

var encode = lzw.encode(buffer);
console.log(encode);

var decode = lzw.decode(buffer);
console.log(decode);

```

## API

### encode(value)

encoding string value and return string encoded

### decode(value)

decoding string value and return string decoded

## AngularJS integration

Under node-lzw-install-path/angular there is lzw.js, port of this library for AngularJS.
Follow example of use.

In your html file put

```html
<script src="path/lzw.js" type="text/javascript"></script>
```

In your angular controller file put

```js
var app = angular.module('app', ['lzw']);

app.controller('myController', function($scope, lzw) {
	...
	var encode = lzw.encode(...);
	...
	var decode = lzw.decode(...);
	...
}
```

## Contributors

- [Marco Murdocca aka `hormander`](https://github.com/hormander)
