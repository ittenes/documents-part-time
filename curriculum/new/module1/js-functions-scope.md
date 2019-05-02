# JS Function and Scope

## Lecture Notes

> #resource LU
- [LU - JS Functions](http://learn.ironhack.com/#/learning_unit/3020)

> #concept function

- black box metaphor (algebra function)
- name is verbSomething
- convention is camelCase
- `function addNumbers(p1, p2) { return p1 + p2 }`

> #concept abstraction
> #concept function call

- `function addNumbers(p1, p2) { console.log(p1 + p2); }`

> #concept call arguments

```js
function doFoo(a, b) { console.log(a, b) }
doFoo(1);
function doFoo(a, b) { console.log(arguments) }
doFoo(1, 2, 3);
```
- addNumbers(1, 2)
- addNumbers(1, 2, 3)
- addNumbers('foo')

> #concept return value

```js
var x = doFoo();
var y = addNumbers(1, 2);
console.log(x);
console.log(y);
```

## Quick Demo

> #concept scope

- var num = 5;
- function addFive(p1) { var x = 1; return p1 + x + 4 }
- addFive();
- console.log(p1);

> #concept hoisting
- sum(2, 4)
- function sum(a, b) { return a + b }

> #concept return statement

- return nothing? return undefined
- return statements in control structures
- multiple return statement

> mantra: code happens

- close laptops
- let's talk about time

> #concept call stack

- breakpoint
- show call stack


```js
function bar(times) {
  console.log('I am bar, I was called', times, 'times');
}

function foo(count) {
  debugger;
  console.log('I am foo');
  for (var ix = 1; ix <= count; ix++) {
    bar(ix);
    console.log('I called bar', ix, 'times');
  }
}

foo(3);
```

> #concept closure

```js
function addNums(a, b) {
  return a + b;
}

function makeFunctionThatAddsY(y) {
  return function (x) {
    return addNums(x, y);
  }
}

var addFive = makeFunctionThatAddsY(5);

addFive(100);
```

> #concept callback

```
function doSomething() {
  console.log('1 sec later');
}
console.log('before');
window.setTimeout(doSomething, 1000)
console.log('after');
```

> #concept anonymous function

window.setTimeout(function () {
  console.log('1 sec later');
}, 1000);

- show in [cheat-sheet](https://github.com/ironhack/bcn-webdev-cheatsheet/tree/master/m1#js-concepts)

> #adaptive
- Review: callback
- Review: anonymous
- [Advanced] Lecture: JS Function + Context
- [Advanced] Lecture: JS Closures + Scope
- [Advanced] Lecture: JS Functional programming, higher order functions

## Activity 

### Role play debugger

- check photo
- @todo - add notes, follow pic

### JS Diagram

- (statement, expression, assignment, declaration, function, parameters, return, scope, call, arguments)