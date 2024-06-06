# react-compiler-runtime-polyfill

[![NPM version][npm-version-src]][npm-version-href]
[![bundle][bundle-src]][bundle-href]
[![JSDocs][jsdocs-src]][jsdocs-href]
[![License][license-src]][license-href]

This is a simple polyfill for react-compiler-runtime, designed to provide developers who cannot upgrade to React 19 at the moment with the ability to use react-compiler.

## Usage

Configure the `runtimeModule` field for your Babel plugin:

```js
// babel.config.js
module.exports = function (api) {
  return {
    plugins: [
      [
        'babel-plugin-react-compiler',
        {
          runtimeModule: 'react-compiler-runtime-polyfill'
        }
      ]
    ]
  }
}
```

That`s all!

## Credit

https://gist.github.com/poteto/37c076bf112a07ba39d0e5f0645fec43

## License

[MIT](./LICENSE) License © 2023 [Riri](https://github.com/Daydreamer-riri)

[npm-version-src]:https://img.shields.io/npm/v/react-compiler-runtime-polyfill?style=flat&colorA=080f12&colorB=1fa669
[npm-version-href]:https://www.npmjs.com/package/react-compiler-runtime-polyfill
[bundle-src]: https://img.shields.io/bundlephobia/minzip/react-compiler-runtime-polyfill?style=flat&colorA=080f12&colorB=1fa669&label=minzip
[bundle-href]: https://bundlephobia.com/result?p=react-compiler-runtime-polyfill
[license-src]: https://img.shields.io/github/license/daydreamer-riri/react-compiler-runtime-polyfill.svg?style=flat&colorA=080f12&colorB=1fa669
[license-href]: https://github.com/daydreamer-riri/react-compiler-runtime-polyfill/blob/main/LICENSE
[jsdocs-src]: https://img.shields.io/badge/jsdocs-reference-080f12?style=flat&colorA=080f12&colorB=1fa669
[jsdocs-href]: https://www.jsdocs.io/package/react-compiler-runtime-polyfill
