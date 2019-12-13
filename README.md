# fastify-plugin-load

Configure the list of plugins to register

## Install

```
npm i fastify fastify-plugin-load
```

## Example

```js
'use strict'

const Fastify = require('fastify')
const PluginLoad = require('fastify-plugin-load')

const fastify = Fastify()

fastify.register(PluginLoad, [
  'fastify-helmet',
  'fadtify-sensible',
  './plugins/local'
])

fastify.listen(3000)
```

## License

MIT
