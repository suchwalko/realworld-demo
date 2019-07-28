# Realworld Demo

Attempt to recreate https://demo.realworld.io (or https://demo.productionready.io) based on webpack starter, javascript, webcomponents.

## Endpoints

[Postman environment](doc/Conduit.postman_environment.json)
[Postman collection](doc/Conduit.postman_collection.json)

## Installation

```
npm install
```

## Start Dev Server

```
npm start
```

## Build Prod Version

```
npm run build
```

## Features:

* ES6 Support via [babel](https://babeljs.io/) (v7)
* SASS Support via [sass-loader](https://github.com/jtangelder/sass-loader)
* Linting via [eslint-loader](https://github.com/MoOx/eslint-loader)

When you run `npm run build` we use the [mini-css-extract-plugin](https://github.com/webpack-contrib/mini-css-extract-plugin) to move the css to a separate file. The css file gets included in the head of the `index.html`.
