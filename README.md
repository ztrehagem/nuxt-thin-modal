# @ztrehagem/nuxt-thin-modal

This plugin brings `$modal` of [vue-thin-modal](https://github.com/ktsn/vue-thin-modal) into store and context.

## Installation

```
$ npm install @ztrehagem/nuxt-thin-modal
```

## Usage

Edit your `nuxt.config.js`.

```js
module.exports = {
  plugins: [
    '@ztrehagem/nuxt-thin-modal'
  ]
}
```

Then you can access `$modal` in components, stores and context.

```js
// in components and store
this.$modal

// via context object
context.app.$modal
```

Note that, the _auto installing_ is disabled in this plugin.
In other words, you must mount `<modal-portal>` component manually. (see [Manually mount portal](https://github.com/ktsn/vue-thin-modal#manually-mount-portal))
