# esbuild-plugin-markdown

Import markdown files with `esbuild`, using [marked](https://github.com/markedjs/marked).

## Install

```sh
yarn add -D esbuild-plugin-markdown
```

or

```sh
npm i -D esbuild-plugin-markdown
```

## Usage

Add it to your esbuild plugins list:

```js
const esbuild = require("esbuild");
const { markdownPlugin } = require("esbuild-plugin-markdown");

esbuild.build({
  ...
  plugins: [
    markdownPlugin()
  ]
  ...
});
```

## Options

You can add your own custom configuration of options to `esbuild-plugin-markdown`:

```js
markdownPlugin({
  // options
});
```

### `markedOptions`

Custom [marked](https://github.com/markedjs/marked) options.
