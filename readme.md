# metalsmith-sense

> A batteries-included distribution of metalsmith available as a plugin.

[![Status](https://travis-ci.org/rstacruz/metalsmith-sense.svg?branch=master)](https://travis-ci.org/rstacruz/metalsmith-sense "See test builds")

[Metalsmith] is a very useful static-site generator with almost all functionality provided by plugins. Most of the time, you will need the same set of functionality out of a site builder:

* CSS:
  * compile using a modern pre-processor when needed. (*.sass, *.styl)
  * don't worry about vendor prefixes. (autoprefixer)
  * compress in production.
* HTML:
  * compile from modern templating languages. (handlebars, jade)
  * support for layout templates. (layouts/)
  * support for partials. (partials/)
* JavaScript:
  * a reasonable build/concat system.
  * transpile using modern babel.
  * compress in production.

<br>

## Quick start

```js
npm init
npm install --save metalsmith metalsmith-sense
npm install --save-dev metalsmith-start
wget "https://raw.githubusercontent.com/rstacruz/metalsmith-sense/master/example/metalsmith.js" -O metalsmith.js
```

Update `package.json`:

```js
...
"scripts": {
  "prepublish": "node metalsmith.js",
  "start": "metalsmith-start"
}
```

Run:

``` sh
npm run prepublish  # build output (production)
npm run start       # start server (development)
```

[Metalsmith]: http://metalsmith.io/
