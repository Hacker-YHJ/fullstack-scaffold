# generator-zero [![NPM version][npm-image]][npm-url] [![Build Status][travis-image]][travis-url] [![Dependency Status][daviddm-image]][daviddm-url] [![Coverage percentage][coveralls-image]][coveralls-url]

> A simple frontend scaffold using coffeescript, pug, stylus, webpack, gulp

## Features

- pug -> html, coffeescript -> javascript, stylus -> css
- use webpack to bundle npm dependencies
- inline css into html
- inline assets as data url
- utilize webpack dev server, hot reload and auto refresh when anything changes
- utilize proxy middleware, good for debugging with existing API

## Folder Structure and Name Convention

```
src
├── coffee
    ├── main.coffee
    └── _dependency.coffee
├── pug
    ├── index.pug
    └── _dependency.pug
├── stylus
    └── index.pug
├── miscellaneous
    ├── robots.txt
    └── favicon.png
└── assets
    └── images
dist
├── index.html
├── robots.txt
├── favicon.png
└── assets
    └── images
```

All coding should happen in `src` folder and all things will be compiled into `dist` folder.
Files in `coffee` and `pug` folder will be compiled if they are not preceeded with an underscore.

## Installation

First, install [Yeoman](http://yeoman.io) and generator-zero using [npm](https://www.npmjs.com/) (we assume you have pre-installed [node.js](https://nodejs.org/)).

```bash
npm install -g yo
npm install -g generator-zero
```

Then generate your new project:

```bash
yo zero
```

## Gulp Tasks

- gulp serve: run the dev server on port 5000
- gulp dist: compile all things into `dist` folder

## Getting To Know Yeoman

 * Yeoman has a heart of gold.
 * Yeoman is a person with feelings and opinions, but is very easy to work with.
 * Yeoman can be too opinionated at times but is easily convinced not to be.
 * Feel free to [learn more about Yeoman](http://yeoman.io/).

## License

MIT © [Thomas Yang](http://thomas-yang.me)


[npm-image]: https://badge.fury.io/js/generator-zero.svg
[npm-url]: https://npmjs.org/package/generator-zero
[travis-image]: https://travis-ci.org/Hacker-YHJ/generator-zero.svg?branch=master
[travis-url]: https://travis-ci.org/Hacker-YHJ/generator-zero
[daviddm-image]: https://david-dm.org/Hacker-YHJ/generator-zero.svg?theme=shields.io
[daviddm-url]: https://david-dm.org/Hacker-YHJ/generator-zero
[coveralls-image]: https://coveralls.io/repos/Hacker-YHJ/generator-zero/badge.svg
[coveralls-url]: https://coveralls.io/r/Hacker-YHJ/generator-zero
