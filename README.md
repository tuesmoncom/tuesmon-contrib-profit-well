Tuesmon Contrib Profit Well
=========================

[![Kaleidos Project](http://kaleidos.net/static/img/badge.png)](https://github.com/kaleidos "Kaleidos Project")
[![Managed with Tuesmon.com](https://img.shields.io/badge/managed%20with-TUESMON.io-709f14.svg)](https://manage.tuesmon.com/project/tuesmon/ "Managed with Tuesmon.com")

The Tuesmon plugin to add profilt well retain snippet.

Installation
------------
### Production env

#### Tuesmon Front

Download in your `dist/plugins/` directory of Tuesmon front the `tuesmon-contrib-profit-well` compiled code (you need subversion in your system):

```bash
  cd dist/
  mkdir -p plugins
  cd plugins
  svn export "https://github.com/tuesmoncom/tuesmon-contrib-profit-well/branches/stable/dist"  "profit-well"
```

Include in your `dist/conf.json` in `profitWellToken` the Profit Well token and in the `contribPlugins` list the value `"/plugins/profit-well/profit-well.json"`:

```json
...
    "profitWellToken": "XXXXXXXXXXXXXXXXXXXXXXXX",
    "contribPlugins": [
        (...)
        "/plugins/profit-well/profit-well.json"
    ]
...
```

### Dev env

#### Tuesmon Front

After clone the repo link `dist` in `tuesmon-front` plugins directory:

```bash
  cd tuesmon-front/dist
  mkdir -p plugins
  cd plugins
  ln -s ../../../tuesmon-contrib-profit-well/dist profit-well
```

Include in your `dist/conf.json` in `profitWellToken` the Profit Well token and in the `contribPlugins` list the value `"/plugins/profit-well/profit-well.json"`:

```json
...
    "profitWellToken": "XXXXXXXXXXXXXXXXXXXXXXXX",
    "contribPlugins": [
        (...)
        "/plugins/profit-well/profit-well.json"
    ]
...
```

In the plugin source dir `tuesmon-contrib-profit-well` run

```bash
  npm install
```
and use:

- `gulp` to regenerate the source and watch for changes.
- `gulp build` to only regenerate the source.

