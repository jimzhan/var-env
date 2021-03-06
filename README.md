# yo-env

Structure your npm scripts better via `NODE_ENV`

[![build](https://travis-ci.org/jimzhan/yo-env.svg?branch=master)](https://travis-ci.org/jimzhan/yo-env)
[![npm version](https://badge.fury.io/js/yo-env.svg)](https://www.npmjs.com/package/yo-env)
[![JavaScript Style Guide](https://camo.githubusercontent.com/387caee7992b38dcac6cb23f87abf0ba139d7101/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f636f64652532307374796c652d616972626e622d626c75652e737667)](https://github.com/airbnb/javascript)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)
[![npm downloads](https://img.shields.io/npm/dt/yo-env.svg)](https://www.npmjs.com/package/yo-env)


## Install

```shell
npm install yo-env
```


## WHAT?

Cross-platform supplement for your npm scripts.


## HOW?

```
// package.json

{
  "scripts": {
    "start": "yo-env",

    /* --- invoked when `NODE_ENV=development` (default). --- */
    "start:development": "nodemon --exec babel-node --inspect src/index.js",

    /* --- invoked when `NODE_ENV=production`. --- */
    "start:production": "node --require esm src/index.js"
  }
}
```

### License

> MIT License 2018 © Jim Zhan
