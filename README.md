# dora-plugin-lutool-build


dora plugin for webpack.


[![NPM version](https://img.shields.io/npm/v/dora-plugin-lutool-build.svg?style=flat)](https://npmjs.org/package/dora-plugin-lutool-build)
[![NPM downloads](http://img.shields.io/npm/dm/dora-plugin-lutool-build.svg?style=flat)](https://npmjs.org/package/dora-plugin-lutool-build)


----

## Usage

```bash
$ dora --plugins lutool-build
```

with options:

```bash
$ dora --plugins lutool-build?publicPath=/${npm_pkg_name}&verbose
```

with options in Object:

```bash
$ dora --plugins lutool-build?{"watchOptions":{"poll":true}}
```

### Options

- `cwd` -- default from dora
- `publicPath` -- default '/', http://webpack.github.io/docs/configuration.html#output-publicpath
- `config` -- default 'webpack.config.js'
- `verbose` -- more logs
- `disableNpmInstall` -- disable NpmInstallPlugin
- `physcisFileSystem` -- write output files to disk 

And other webpack options, like `watchOptions`, `headers`, `stats`, ...


## Plugins

- `lutool-build.updateWebpackConfig` -- update webpack config for development

