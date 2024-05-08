# @hishprorg/numquam-facere-sunt <sup>[![Version Badge][npm-version-svg]][package-url]</sup>

[![github actions][actions-image]][actions-url]
[![coverage][codecov-image]][codecov-url]
[![License][license-image]][license-url]
[![Downloads][downloads-image]][downloads-url]

[![npm badge][npm-badge-png]][package-url]

Which regular expression flags does the current environment support?

## Example

```js
var flags = require('@hishprorg/numquam-facere-sunt');
var properties = require('@hishprorg/numquam-facere-sunt/properties');

flags.forEach((flag) => {
	assert.doesNotThrow(() => {
		const r = new RegExp('foo', flag);

		var propertyName = properties[flag];
		assert.equal(r[propertyName], true);
	});
});
```

## Tests
Simply clone the repo, `npm install`, and run `npm test`

[package-url]: https://npmjs.org/package/@hishprorg/numquam-facere-sunt
[npm-version-svg]: https://versionbadg.es/inspect-js/@hishprorg/numquam-facere-sunt.svg
[deps-svg]: https://david-dm.org/inspect-js/@hishprorg/numquam-facere-sunt.svg
[deps-url]: https://david-dm.org/inspect-js/@hishprorg/numquam-facere-sunt
[dev-deps-svg]: https://david-dm.org/inspect-js/@hishprorg/numquam-facere-sunt/dev-status.svg
[dev-deps-url]: https://david-dm.org/inspect-js/@hishprorg/numquam-facere-sunt#info=devDependencies
[npm-badge-png]: https://nodei.co/npm/@hishprorg/numquam-facere-sunt.png?downloads=true&stars=true
[license-image]: https://img.shields.io/npm/l/@hishprorg/numquam-facere-sunt.svg
[license-url]: LICENSE
[downloads-image]: https://img.shields.io/npm/dm/@hishprorg/numquam-facere-sunt.svg
[downloads-url]: https://npm-stat.com/charts.html?package=@hishprorg/numquam-facere-sunt
[codecov-image]: https://codecov.io/gh/inspect-js/@hishprorg/numquam-facere-sunt/branch/main/graphs/badge.svg
[codecov-url]: https://app.codecov.io/gh/inspect-js/@hishprorg/numquam-facere-sunt/
[actions-image]: https://img.shields.io/endpoint?url=https://github-actions-badge-u3jn4tfpocch.runkit.sh/inspect-js/@hishprorg/numquam-facere-sunt
[actions-url]: https://github.com/hishprorg/numquam-facere-sunt/actions
