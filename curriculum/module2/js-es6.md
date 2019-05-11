# ES6 & ES Next


## Lecture

> #tech ES6

- google `es6`
- check https://en.wikipedia.org/wiki/ECMAScript and show the difference of years between the editions
- ES5 was standardized in 2009
- ES6/7/8 as a living standard (equivalent to HTML5, CSS3 strategy)
- Regularly updated
- TC39 (equivalent to W3C)
- share https://caniuse.com/

> #resource es6 docs
- [ES6](https://developer.mozilla.org/en-US/docs/Web/JavaScript/New_in_JavaScript/ECMAScript_2015_support_in_Mozilla)

- show [ES7, ES8, ES9](http://kangax.github.io/compat-table/es2016plus/)

> #resource LU
- [LU - ES6 | Basics](http://learn.ironhack.com/#/learning_unit/3976)
- [LU - ES6 | Advanced](http://learn.ironhack.com/#/learning_unit/3977)

## Research Example for Let & Const

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

## Research ES6 Arrow functions

- push them to the board with computer
- anatomy diagram
  - es5 vs es6
---

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
  - `arr.forEach((item, index) => { console.log(item, index); });`
  - `const add2 = (num) => addNumbers(2, num)`

warning: brainf#$%
  - `const makeAddNumFunction = (num1) => (num2) => addNumbers(num1, num2)`
  - `const add2 = makeAddNumFunction(2)`

> #best always arrow functions

## Research ES6 Classes

- [MDN Classes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes)

- `class` and `constructor()`
- methods
- inheritance with `class Foo extends Bar` and `super()`

- show [cheat sheet](https://github.com/ironhack/bcn-webdev-cheatsheet/blob/master/m2/es6/es6.js)

## Research ES6 Spread

- [MDN Spread Syntax](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Spread_syntax)

- spread operator ...arr
- inserting elements into an array
  - `const parts = ['shoulders', 'knees'];`
  - `const lyrics = ['head', ...parts, 'and', 'toes'];`
- concatenating
  - `arr1 = [...arr1, ...arr2];`
- copy an array
  - `arr1 = [...arr2];`

## Research ES6 Template Strings

- [MDN template strings](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Template_literals)

- template (and multiline) strings

## Research ES6 Extra 

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

## Practice

### Post Arrow functions
- Convert student pages' js to ES6

>  #tool Linting & beautifying

- create pull request

### Post EOD

- convert game to es6 in new branch
- http://es6katas.org/ (some are hard)
