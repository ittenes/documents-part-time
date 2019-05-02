# NodeJS

## Lecure notes

> #tech Node.js

> #resource LU
- [LU Node Intro](http://learn.ironhack.com/#/learning_unit/3985)

> #resource Node.js
- [Node.js docs](https://nodejs.org/dist/latest-v10.x/docs/api/)

- main use case: http server
- other languages generally used for same purpose: ruby, php, .net, java, go, scala

- **IT'S NOT A FRAMEWORK!**
  - runtime environment for running javascript in the backend (v8 engine)
  - app can be an http server (runs "forever")
  - runs javascript, same as browser (but no window, no DOM)
  - node callbacks convention (err, result) => { ... }
  - has some built-in modules like `fs`, `process`, `path` and `http`

- other Node.js use cases, not only http servers
  - node-sass, webpack, gulp, grunt
  - babel
  - eslint
  - [image processing](https://www.youtube.com/watch?v=iW6eWvxpfvc)
  - [webscrapping cherio](https://www.youtube.com/watch?v=eUYMiztBEdY)
  - [webscrapping puppeteer](https://github.com/GoogleChrome/puppeteer)
  - [testing w/ nightwatch.js](https://www.youtube.com/watch?v=zzofkNaoPYE)
  - [flying robots](http://www.nodecopter.com/)
  - [canvas art](https://mattdesl.svbtle.com/generative-art-with-nodejs-and-canvas)
  - [watering your plants](https://www.instructables.com/id/IoT-NFT-Aquaponic-System-Controler-with-WebApp-Int/)

## Code Along

- install node
- build a quote generator w/ functions + array modules + chalk

- the console
  - `node`

- running an app
  - `touch app.js`
```javascript
console.log('done!');
```
  - `node app.js`

> #concept NPM Packages

- [NPM](http://npmjs.org)
- npm init (new projects only)
- npm install (after cloning existing project)
- npm install --save package-name
- npm install --save-dev package-name
- npm install -g package-name (may require sudo)
- package.json (every node project needs one)
- always add "node_modules" to .gitignore

> #concept CommonJS Modules

- every js file is a module
- every file has it's own scope (no global scope)
- npm packages are also modules
- for our files:
  - in `folder/mymodule.js`, to define what it exports
    - `module.exports = ...`
  - in another file use relative path to require it
    - `const mymodule = require('./folder/mymodule')`
- for npm packages:
  - const express = require('express')

- create repo in github for the codealong: https://github.com/tawebbcn/node-intro
  - remember the gitignore
- made the cohort clone the repo of the person to the right for them to find out that it won't work
  - introduce npm install


## Practice

- Intro node (mocha) @todo add notes and link