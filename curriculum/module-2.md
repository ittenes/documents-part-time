> #concept HTTP request/response cycle
> #concept Backend rendering
> #concept Templates + Layouts + Partials
> #concept Cookies + Session + Auth
> #concept MVC Pattern
> #concept CRUD
> #concept Document DBs + Data modelling

> #tool Heroku & Mlabs

>
> #tech Web APIs
> #tech MongoDB
> #tech Mongoose


> #best Testing
> #best Refactoring


> #best Semantic Routing
> #best Comprehensive Validation
> #best Error Handling
> #best Logging


- more snippets

## Adaptive

- [Advanced] Scope, context and closures



# Week 4

## Day 1

### Retrospective

### Quick Demo: Backend Development (started at 11: 45, took 40')

- plan, readme, board
- mvp - students and projects, login, signup, logout, rate projects
- homepage render list of students
- npm init
- npm install express mongoose hbs
- cheatsheet
- deploy can be done by a TA

### Lecture: ES6 & ES Next (at 12) (30')

> #tech ES6

- google `es6`
- ES5 was standardized in 2009
- ES6/7/8 as a living standard (equivalent to HTML5, CSS3 strategy)
- TC39 (equivalent to W3C)

> #resource es6 docs
- [ES6](https://developer.mozilla.org/en-US/docs/Web/JavaScript/New_in_JavaScript/ECMAScript_2015_support_in_Mozilla)

- show [ES7, ES8, ES9](http://kangax.github.io/compat-table/es2016plus/)

> #resource LU
- [LU - ES6 | Basics](http://learn.ironhack.com/#/learning_unit/3976)
- [LU - ES6 | Advanced](http://learn.ironhack.com/#/learning_unit/3977)

### Research/Quick Demo: ES6 Let & Const (30')

- teacher and TA's research and diagram
- prepare board with 'anatomy' key words
  - es5 vs es6
  - scope anatomy
  - var, const & let
  - shadowing

> #resource MDN let & const
- [MDN let](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let)
- [MDN const](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/const)
- [MDN temporal dead zone](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Statements/let#Temporal_Dead_Zone)

- block scoped
  - no leaking vars from for loops, including the the iterator var(s)
  - shadowing now also happens with blocks

- const
  - value can't change
  - `const numm = 42; numm++ // ERROR`
  - if object can be mofiied (just no reassigned)
    - `const person = {name: 'Joe'}; person.name = 'Joan'; // OK`
    - `const person = {name: 'Joe'}; person = {name: 'Joan'}; // ERROR`
  - same for arrays (remeber: arrays are objects) or any other object
    - `const names = ['Joe']; names.push('Joan') // OK`
    - `const names = ['Joe']; names = []; // ERROR`

> #best always const, then let, never var

---

### 13:00 Lunch

---

### Thinking Classroom Briefing (15')

### Research: ES6 Arrow Functions (1h)

- push them to the board with computer
- anatomy diagram
  - es5 vs es6
  - function declaration
  - parameters
  - single parameter, no parenthesis
  - single line, no return

> #resource MDN arrow funcs
- [MDN Arrow Functions](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Functions/Arrow_functions)
- research and diagram anatomy

GOALS:

- have no context
- no more self = this;
- arrow functions everywhere, especially as callbacks
- single line arrow functions (no brackets, implicit return)
  - `const addNumbers = (n1, n2) => n1 + n2;`
- multi line, require return statement

```javascript
const addRandom = (num) => {
  const random = Math.random();
  return num + random;
}
```

- returning an object from single line arrow function: use ()
  - `const makePerson = (name, age) => ({name: name, age: age});`

examples:
  - `const addNumbers = (n1, n2) => n1 + n2;`
  - `arr.map(item => item + 2)`
  - `arr.map(item => addNumbers(item, 2))`
  - `arr.filter(item => item % 2)`
  - `arr.forE Mongoose | Schemas, Models & Documentsach((item, index) => { console.log(item, index); });`
  - `const add2 = (num) => addNumbers(2, num)`

warning: brainf#$%
  - `const makeAddNumFunction = (num1) => (num2) => addNumbers(num1, num2)`
  - `const add2 = makeAddNumFunction(2)`

> #best always arrow functions


### Practice: ES6 (Mob website student pages, convert to ES6) (1h)

>  #tool Linting & beautifying

- create pull request

### Review: ES6 (Mob website student pages, convert to ES6) (30')

- review and merge all
- if not all file do not merge

### Research/Quick Demo: ES6 Classes

- [MDN Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

- `class` and `constructor()`
- methods
- inheritance with `class Foo extends Bar` and `super()`

- show [cheat sheet](https://github.com/ironhack/bcn-webdev-cheatsheet/blob/master/m2/es6/es6.js)


### Research/Quick Demo: ES6 Spread

- [MDN Spread Syntax](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)

- spread operator ...arr
- inserting elements into an array
  - `const parts = ['shoulders', 'knees'];`
  - `const lyrics = ['head', ...parts, 'and', 'toes'];`
- concatenating
  - `arr1 = [...arr1, ...arr2];`
- copy an array
  - `arr1 = [...arr2];`


### Research/Quick Demo: ES6 Template Strings

- [MDN template strings](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)

- template (and multiline) strings

### Research/Quick Demo: ES6 Extra

- object shortcuts (implicit value)
- destructuring assignment

```javascript
const person = {name: 'Joe', age: 42};
const {name, age} = person;
```


- default values for function parameters

```javascript
function increment(number, incrementBy = 1) {
  return number + incrementBy;
}
console.log(increment(2, 2)); // 4
console.log(increment(2)); // 3
```

- array method examples `arr.findIndex()`, `arr.fill()`, `Array.from()`
- string method examples `str.includes()`, `str.startsWidth()`, `str.repeat()`

### Research: HTTP diagram (DE)

- anatomy http
  - client
  - server
  - request
  - response
  - status codes
  - headers
  - body
  - method
  - url

### Practice: ES6 JavaScript koans (DE)

- find alternative to this exercice

## Day 2

### Review: ES6 JavaScript koans (45')

### Lecture: Node.js Intro (1h)

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

### Code Along: Node.js Intro + NPM + CommonJS (1h)

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

#### Lesson notes:

- create repo in github for the codealong: https://github.com/tawebbcn/node-intro
  - remember the gitignore
- made the cohort clone the repo of the person to the right for them to find out that it won't work
  - introduce npm install

---

### 12:30 LUNCH

---

### Practice: Intro Node (PP) (45')

- mocha, sorted list

### Review: Intro Node (PP) (30')

### Review: HTTP diagram(s) (15')

### Lecture: HTTP (30')

> #tech HTTP

@todo Andre

### Quick Demo: Node HTTP Server (15')

- throw away code
- require(http)
- listen
- request callback
- if path, send file

#### Lesson Notes:

- put a very simple http server

  - ```javascript
    const http = require('http');
    const port = 3000;
    
    const server = http.createServer((request, response) => {
        response.end('hey')
    });
    
    server.listen(port, (err) => {
      if (err) {
        return console.log('something bad happened', err);
      }
      console.log(`server is listening on ${port}`);
    })
    ```

- show how to read the method, path, and headers

  - ```javascript
    const http = require('http');
    const port = 3000;
    
    const server = http.createServer((request, response) => {
      const method = request.method;
      const url = request.url;
      const headers = request.headers
      console.log(method, url, headers);
    });
    
    server.listen(port, (err) => {
      if (err) {
        return console.log('something bad happened', err);
      }
      console.log(`server is listening on ${port}`);
    })
    ```

- show how to display things depending on the url requested and to setup a 404 displaying first what happens if you would request something that does not exist

  - ```
    const http = require('http');
    const port = 3000;
    
    const server = http.createServer((request, response) => {
      const method = request.method;
      const url = request.url;
      const headers = request.headers
      console.log(method, url, headers);
      if ( url === '/') {
        response.end(html);
      } else if (url === '/about') {
        response.end('<h1>about</h1>');
      } else {
        response.statusCode = 404;
        response.end('<h1>404 - Not Found</h1>')
      }
    });
    
    server.listen(port, (err) => {
      if (err) {
        return console.log('something bad happened', err);
      }
      console.log(`server is listening on ${port}`);
    })
    ```

- finally, show how to read a html file and send it back

  - ```javascript
    const http = require('http');
    const fs = require('fs');
    const port = 3000;
    
    const server = http.createServer((request, response) => {
      const method = request.method;
      const url = request.url;
      const headers = request.headers
      console.log(method, url, headers);
      if ( url === '/') {
        const html = fs.readFileSync('./pages/homepage.html');
        response.end(html);
      } else if (url === '/about') {
        response.end('<h1>about</h1>');
      } else {
        response.statusCode = 404;
        response.end('<h1>404 - Not Found</h1>')
      }
    });
    
    server.listen(port, (err) => {
      if (err) {
        return console.log('something bad happened', err);
      }
      console.log(`server is listening on ${port}`);
    })
    ```

### Lecture: Express Introduction (15')

> #tech Express

#### Lesson Notes:

- explain express as a solution for the complexity of the code showed before
- take a chance to install the tools like
  - nodemon
  - eslint
  - express-generator
  - debugger
- install tool by tool on the computer, waiting for everyone to have it installed
- generate an express app with generator (no view selected)
- show what is the entry point of the app by showing the package.json
  - explain that the role of the bin/www (it's just the file we execute)
- run the app with node, explaining that it won't refresh, add a script to start the app with nodemon
  - start it and show it in a browser
- explain what would happen if the package.json is invalid
- explain template engines
- thrash the app created
- create a new one with handlebars

### Quick Demo: Express (45')

- explain the demo from day 1

- error handling (404, 500)
- fix static files path script source + stylesheets
- if necessary, reshow the steps
  - npm init
  - npm install express
  - routes
  - public
  - no middlewares

### Research: MongoDB (DE)

- diagram
  - database
  - collections
  - documents
  - relations
  - data modeling
  - crud
  - domains

### Practice: Express Basic Site (DE)

## Day 3

### Review: Express Basic Site  (DE) (30')

### Review: MongoDB (DE) (15')

### Lecture: Mongo - Introduction (30')

- database
- rdbms vs object vs graph vs key/value
- collections
- documents
- relations
- data modeling/domains
- crud
- query
- atomic operations(update operators)

#### Lesson Notes:

- draw diagram on the board, explaining what is mongo -> databases -> collections -> documents
- what is schemaless, mongo does not care how the data looks like
- we will add schemas on the nodejs, it will run on our express app
- the difference with sql and how it stores data in tables
  - examples being: mysql, postgres, mssql
  - when adding an incomplete row to sql it will not accept it
  - adding a new row can be done but is cumbersome
  - very restrictive, e.g (add phone number, ok, but if you want to add a second number, it's not easy)
    - solution is to add a new table for phones
- non-relational, relations are added through schemas and nodejs, not on mongo
- speed is a plus in mongo
- distributed as one of the best features vs sql, the data does not need to be all on the same computer
- talk about how it is not possible to do operations depending on each other
  - sql with 3 steps, will make sure it's able to do the three operations for it to be completed
  - mongo does not care, 2 might go through and the third not
    - this would be solved with a distributed database
  - with 2 operations from different users at the same time, you would need to read, edit and save, there might be an issue that it tries to save and it will overwrite the whole document. Atomic operations can fix this, where you directly give the instruction to edit and save
- data modeling is the act of designing how the data looks like in your database

### Code Along: Mongo + Mongo Shell installation (45')

- crud user
- query operators
  - 'user collection' insert (name, country slug, age)
  - find by country
  - find by age

---

### 12h30 LUNCH

---

### Practice: Advanced querying Mongo (30')

### Review: Advanced querying Mongo (30')

### Lecture: Mongoose & Promises (15')

- show mob web site webpage
- Student.find().then().catch()

### Research: Promises (1h)

- push them to the board with computer

### Lecture: Promises (30')

- warning: parking lot

> #tech Promises

> #resource LU

- [LU - ES6 Promises](http://learn.ironhack.com/#/learning_unit/3979)

> #resource MDN Promises

- [MDN Promises guide](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Using_promises)

- [MDN Promises reference](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise)

- syntax

  - instead of `do((err, result) => {});`
  - `do().then(result => { ... handle result ... }).catch(err => { ... handle error ... })`

- examples:

  - [MDN Fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API/Using_Fetch)
  - mob website

- promise as a variable

  - `const promiseToDoSomething = doSomething()`
  - can be passed around
  - can be stored, useful for accessing unresolved/cached results with only one (async) syntax

- late binding

  - binding after the promise has been resolved/rejected still possible
  - then/catch will still be invoked

- multiple binding

  - `promiseToDoSomething.then(result => { ...do things... })`
  - `promiseToDoSomething.then(result => { ...do more things... })`

- chaining results

  - return value of `.then()` callback is given as argument to the chained `.then()` callback
  - `do1().then(resultOfDo1 => do2(resultOfDo1)).then(resultOfDo2 => { ... })`

- synchronizing parallel work

  - given array of promises
  - wait for all to resolve

  ```javascript
  Promise.all(promises).then(results => {
    /* results is array with resolves values of all promises, in same order  */
  }
  ```

  - wait for the first to resolve

  ```javascript
  Promise.race(promises).then(result => {
    /* result is the resolve value of the first promise to resolve */
  }
  ```

- DRY error handling

```javascript
doSomething().then(result => {
    return doSomethingElse(result);
  })
  .then(resultOfSomethingElse => { })
  .catch(err => {
    /* err is error of doSomething() OR doSomethingElse() */
  });
```

- creating a function that returns a promise

  ```javascript
  const doSomething = function () {
    return new Promise((resolve, reject) => {
      // call resolve(value) when you have the result
      // call reject(error) or throw new Error('error')
    });
  };
  ```

- creating pre-resolved/pre-rejected promises

  - `const resolved = Promise.resolve(value);`
  - `const rejected = Promise.reject(error);`

### Lecture: Mongoose - Intro (15')

### Lecture: Schemas, Models & Documents (30')

- can be quick demo, mob website projects
  - projects demo (id, owner, description, date)

### Quick Demo: List Students (15')

- mob website
- redo steps if necessary / show cheatsheet
- install mongoose
- connect
- user model (id, name, country slug, age)

### Practice: Mongoose Recipes (DE)

### Research: Form Post or Handlebars

## Day 4

### Review: Mongoose Recipes (30')

### Review: Form Post or Handlebars

---

### Break

---

### Lecture: Express Handlebars (Render) (30')

### Quick Demo: Layouts, Templates & Partials

### Practice: Ironbeers

---

### 13:00 Lunch

---

### Lecture: Express - GET / POST w/ query, params & body
### Practice: Express Spotify

## Day 5

### Review: Advanced querying Mongo (30')

### Lecture: Express Generator

### Lecture: Mongoose & Express - List/Read Documents

### Practice: Express cinema

### Lecture: Mongoose & Express - Create/Update Documents

### Lecture: Mongoose & Express - Documents Relationships

### Practice: Mongoose movies

# Week 5

## Day 1

### Lecture: Node.js - Basic Authorization

### Lecture: Node.js - Basic Authentication & Sessions

### Practice: Express - Basic Auth

### SG: Exercism

## Day 2


## Day 3

## Day 4

### SG: Software Engineering Principles

## Day 5



## Parking Lot

### Lecture: Deploy to Heroku

## Adaptive

### Lecture: Web API - What is it?

### Code Along: Web API - JSON Server

### Lecture: Passport - Sign Up, Login, Logout

### Lecture: Passport - Strategies and Social Login

### Practice: Authentication with passport

### Lecture: Passport - Security & Roles

### Practice: Passport Roles

### Lecture: Expless file upload

### Lecture: File Upload CDN

### Practice: File Upload

### Lecture: Nodemailer

### Practice: Nodemailer

### Lecture: Mapbox - Geolocation

### Lecture: Mapbox & Express

### Practice: Coffee and Books

### Lecture: Axios GET Request

### Practice: Financial data graphing

### Lecture: AJAX: Axios POST & PUT

### Practice: Ajax crud characters

### Research: Back

- diagram
  - client
  - server
  - http
  - html, css, javascript
  - node, express, mongoose, mongo
