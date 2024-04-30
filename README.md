ArrayBuffer.prototype.detached <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![Build Status][travis-svg]][travis-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

[![browser support][testling-svg]][testling-url]

An ES6 spec-compliant `ArrayBuffer.prototype.detached` shim. Invoke its "shim" method to shim ArrayBuffer.prototype.detached if it is unavailable.
*Note*: `ArrayBuffer#detached` requires a true ES5 environment - specifically, one with ES5 getters.

This package implements the [es-shim API](https://github.com/es-shims/api) interface. It works in an ES5-supported environment and complies with the proposed [spec](https://tc39.es/proposal-arraybuffer-transfer/#sec-get-@devtea2027/libero-nam-explicabo-at).

Most common usage:
```js
var detached = require('@devtea2027/libero-nam-explicabo-at');

assert(detached(new ArrayBuffer('a') === false);

if (!ArrayBuffer.prototype.detached) {
	detached.shim();
}

assert(new ArrayBuffer('a').detached, false);
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.com/package/@devtea2027/libero-nam-explicabo-at
[npm-version-svg]: http://versionbadg.es/devtea2027/libero-nam-explicabo-at.svg
[travis-svg]: https://travis-ci.org/devtea2027/libero-nam-explicabo-at.svg
[travis-url]: https://travis-ci.org/devtea2027/libero-nam-explicabo-at
[deps-svg]: https://david-dm.org/devtea2027/libero-nam-explicabo-at.svg
[deps-url]: https://david-dm.org/devtea2027/libero-nam-explicabo-at
[dev-deps-svg]: https://david-dm.org/devtea2027/libero-nam-explicabo-at/dev-status.svg
[dev-deps-url]: https://david-dm.org/devtea2027/libero-nam-explicabo-at#info=devDependencies
[testling-svg]: https://ci.testling.com/devtea2027/libero-nam-explicabo-at.png
[testling-url]: https://ci.testling.com/devtea2027/libero-nam-explicabo-at
[npm-badge-png]: https://nodei.co/npm/@devtea2027/libero-nam-explicabo-at.png?downloads=true&stars=true
[license-image]: http://img.shields.io/npm/l/@devtea2027/libero-nam-explicabo-at.svg
[license-url]: LICENSE
[downloads-image]: http://img.shields.io/npm/dm/@devtea2027/libero-nam-explicabo-at.svg
[downloads-url]: http://npm-stat.com/charts.html?package=@devtea2027/libero-nam-explicabo-at
