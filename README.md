# remarkable-mentions [![NPM version](https://img.shields.io/npm/v/remarkable-mentions.svg?style=flat)](https://www.npmjs.com/package/remarkable-mentions) [![NPM downloads](https://img.shields.io/npm/dm/remarkable-mentions.svg?style=flat)](https://npmjs.org/package/remarkable-mentions) [![Build Status](https://img.shields.io/travis/doowb/remarkable-mentions.svg?style=flat)](https://travis-ci.org/doowb/remarkable-mentions)

Transform @ mentions into markdown links.

## Install

Install with [npm](https://www.npmjs.com/):

```sh
$ npm install --save remarkable-mentions
```

## Usage

```js
var mentions = require('remarkable-mentions');
```

## API

### [mentions](index.js#L22)

Remarkable plugin that will turn all @ mentions into a link. This is done just after block tokenizing to ensure that the inline blocks are transformed before links are transformed. This also ensures that @ mentions inside code blocks are not transformed.

**Params**

* `options` **{Object}**: Options to control how the @ mentions are transformed. See [to-mention-link](https://github.com/doowb/to-mention-link) for more options.
* `options.url` **{String}**: Customize the url that is used in the links. Defaults to "https://github.com".
* `returns` **{Function}**: Remarkable plugin function that can be passed to the `.use` method.

**Example**

```js
var md = new Remarkable();
md.use(mentions());
var html = md.render(markdown);
```

## About

### Related projects

* [markdown-link](https://www.npmjs.com/package/markdown-link): Micro util for generating a single markdown link. | [homepage](https://github.com/jonschlinkert/markdown-link "Micro util for generating a single markdown link.")
* [parse-mentions](https://www.npmjs.com/package/parse-mentions): Parse and optionally replace @ mentions from a string of text. | [homepage](https://github.com/doowb/parse-mentions "Parse and optionally replace @ mentions from a string of text.")
* [remarkable](https://www.npmjs.com/package/remarkable): Markdown parser, done right. 100% Commonmark support, extensions, syntax plugins, high speed - all in… [more](https://github.com/jonschlinkert/remarkable) | [homepage](https://github.com/jonschlinkert/remarkable "Markdown parser, done right. 100% Commonmark support, extensions, syntax plugins, high speed - all in one.")
* [to-mention-link](https://www.npmjs.com/package/to-mention-link): Create links from @ mentions. | [homepage](https://github.com/doowb/to-mention-link "Create links from @ mentions.")

### Contributing

Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](../../issues/new).

Please read the [contributing guide](contributing.md) for avice on opening issues, pull requests, and coding standards.

### Building docs

_(This document was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme) (a [verb](https://github.com/verbose/verb) generator), please don't edit the readme directly. Any changes to the readme must be made in [.verb.md](.verb.md).)_

To generate the readme and API documentation with [verb](https://github.com/verbose/verb):

```sh
$ npm install -g verb verb-generate-readme && verb
```

### Running tests

Install dev dependencies:

```sh
$ npm install -d && npm test
```

### Author

**Brian Woodward**

* [github/doowb](https://github.com/doowb)
* [twitter/doowb](http://twitter.com/doowb)

### License

Copyright © 2016, [Brian Woodward](https://github.com/doowb).
Released under the [MIT license](https://github.com/doowb/remarkable-mentions/blob/master/LICENSE).

***

_This file was generated by [verb-generate-readme](https://github.com/verbose/verb-generate-readme), v0.1.30, on September 24, 2016._