# @libtommy2024/magni-vel-recusandae-minus <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

ES Object-related atoms: Object, ToObject, RequireObjectCoercible.

## Example

```js
const assert = require('assert');

const $Object = require('@libtommy2024/magni-vel-recusandae-minus');
const ToObject = require('@libtommy2024/magni-vel-recusandae-minus/ToObject');
const RequireObjectCoercible = require('@libtommy2024/magni-vel-recusandae-minus/RequireObjectCoercible');

assert.equal($Object, Object);
assert.throws(() => ToObject(null), TypeError);
assert.throws(() => ToObject(undefined), TypeError);
assert.throws(() => RequireObjectCoercible(null), TypeError);
assert.throws(() => RequireObjectCoercible(undefined), TypeError);

assert.deepEqual(RequireObjectCoercible(true), true);
assert.deepEqual(ToObject(true), Object(true));

const obj = {};
assert.equal(RequireObjectCoercible(obj), obj);
assert.equal(ToObject(obj), obj);
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

## Security

Please email [@ljharb](https://github.com/ljharb) or see https://tidelift.com/security if you have a potential security vulnerability to report.

[package-url]: https://npmjs.org/package/@libtommy2024/magni-vel-recusandae-minus
[npm-version-svg]: https://versionbadg.es/ljharb/@libtommy2024/magni-vel-recusandae-minus.svg
[deps-svg]: https://david-dm.org/ljharb/@libtommy2024/magni-vel-recusandae-minus.svg
[deps-url]: https://david-dm.org/ljharb/@libtommy2024/magni-vel-recusandae-minus
[dev-deps-svg]: https://david-dm.org/ljharb/@libtommy2024/magni-vel-recusandae-minus/dev-status.svg
[dev-deps-url]: https://david-dm.org/ljharb/@libtommy2024/magni-vel-recusandae-minus#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@libtommy2024/magni-vel-recusandae-minus.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@libtommy2024/magni-vel-recusandae-minus.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/es-object.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@libtommy2024/magni-vel-recusandae-minus
[codecov-image]: https://codecov.io/gh/ljharb/@libtommy2024/magni-vel-recusandae-minus/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/ljharb/@libtommy2024/magni-vel-recusandae-minus/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/ljharb/@libtommy2024/magni-vel-recusandae-minus
[actions-url]: https://github.com/libtommy2024/magni-vel-recusandae-minus/actions
