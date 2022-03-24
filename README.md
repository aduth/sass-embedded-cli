# sass-embedded-cli

Command-line interface for [`sass-embedded`](https://github.com/sass/embedded-host-node) which can be used as a ([mostly](#usage)) drop-in replacement for [`node-sass`](https://github.com/sass/node-sass).

## Installation

Install using `npm`. `sass-embedded` is a peer dependency and must be installed, if not already.

```
npm install sass-embedded-cli sass-embedded
```

## Usage

Usage should match [`node-sass` command-line usage](https://github.com/sass/node-sass#command-line-interface).

Note that `sass-embedded` is not fully compatible with `node-sass`, as it is based on the Dart implementation. In particular, this affects the default `--output-style`, which must be specified as one of the [valid Dart Sass styles](https://sass-lang.com/documentation/cli/dart-sass#style) (`expanded` or `compressed`).

```
node-sass styles.scss --output-style compressed
```

## License

Copyright 2022 Andrew Duthie

Released under the MIT License. See [LICENSE.md](./LICENSE.md).
