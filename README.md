# assemble-render [![NPM version](https://badge.fury.io/js/assemble-render.svg)](http://badge.fury.io/js/assemble-render)

> Plugin for Assemble, Verb, and Gulp to render files.

## Install
## Install with [npm](npmjs.org)

```bash
npm i assemble-render --save
```

## Run tests

```bash
npm test
```

## Usage

```js
var assembleRender = require('assemble-render');
```

## API
### [.renderPlugin](index.js#L31)

Assemble renderer plugin used to render templates passed through the stream.

```js
var assemble = require('assemble');
var renderPlugin = require('assemble-render');
```

### [.render](index.js#L51)

Create a stream that will render files with assemble.

* `options` **{Object}**: Additional options to use.    
* `locals` **{Object}**: Additional locals to pass to the renderer.    
* `returns` **{Stream}**: Stream compatible with Assemble pipelines  

```js
var render = renderPlugin(assemble);
assemble.task('build-posts', function () {
  assemble.src('*.hbs')
    .pipe(render());
});
```


## Contributing
Pull requests and stars are always welcome. For bugs and feature requests, [please create an issue](https://github.com/assemble/assemble-render/issues)

## Author

**Brian Woodward**
 
+ [github/assemble](https://github.com/assemble)
+ [twitter/assemble](http://twitter.com/assemble) 

## License
Copyright (c) 2014 Brian Woodward  
Released under the MIT license

***

_This file was generated by [verb](https://github.com/assemble/verb) on December 11, 2014._