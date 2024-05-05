# @hoangcung1804npm/officiis-debitis-natus <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Is this value a JS Set? This module works cross-realm/iframe, and despite ES6 @@toStringTag.

## Example

```js
var isSet = require('@hoangcung1804npm/officiis-debitis-natus');
assert(!isSet(function () {}));
assert(!isSet(null));
assert(!isSet(function* () { yield 42; return Infinity; });
assert(!isSet(Symbol('foo')));
assert(!isSet(1n));
assert(!isSet(Object(1n)));

assert(!isSet(new Map()));
assert(!isSet(new WeakSet()));
assert(!isSet(new WeakMap()));

assert(isSet(new Set()));

class MySet extends Set {}
assert(isSet(new MySet()));
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@hoangcung1804npm/officiis-debitis-natus
[npm-version-svg]: https://versionbadg.es/inspect-js/@hoangcung1804npm/officiis-debitis-natus.svg
[deps-svg]: https://david-dm.org/inspect-js/@hoangcung1804npm/officiis-debitis-natus.svg
[deps-url]: https://david-dm.org/inspect-js/@hoangcung1804npm/officiis-debitis-natus
[dev-deps-svg]: https://david-dm.org/inspect-js/@hoangcung1804npm/officiis-debitis-natus/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@hoangcung1804npm/officiis-debitis-natus#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@hoangcung1804npm/officiis-debitis-natus.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@hoangcung1804npm/officiis-debitis-natus.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@hoangcung1804npm/officiis-debitis-natus.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@hoangcung1804npm/officiis-debitis-natus
[codecov-image]: https://codecov.io/gh/inspect-js/@hoangcung1804npm/officiis-debitis-natus/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@hoangcung1804npm/officiis-debitis-natus/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@hoangcung1804npm/officiis-debitis-natus
[actions-url]: https://github.com/hoangcung1804npm/officiis-debitis-natus/actions
