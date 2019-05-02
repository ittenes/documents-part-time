# JS Intro

## Lecture

> #tech javascript

> #resource LU
- [LU - Javascript Introduction](http://learn.ironhack.com/#/learning_unit/3012)
- [LU - Conditionals and Loops](http://learn.ironhack.com/#/learning_unit/3013)

> #concept programming
  - Programming is the process of creating a set of instructions that tell a computer how to perform a task.

- google `programming`

> #technology javascript

- google `javascript`
- 1995 (2 years after the Internet)
- ECMAScript
- browser wars part 1
- browser wars part 2
- ES5 (2009) not ES6 (2015)
- no types

> #resource MDN Javascript
- [MDN Javascript guide](https://developer.mozilla.org/bm/docs/Web/JavaScript)
- [MDN Javascript reference](https://developer.mozilla.org/bm/docs/Web/JavaScript)

## Quick Demo

- open MDN developer tools at [Expressions and operators](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Guide/Expressions_and_Operators#Assignment_operators)
- open console on that website

> #concept variable

> #concept declaration

var y;

> #concept assigment

- y = 11;

> #concept expression

- var x = 1932 / y;

> #concept statement

> #concept type
- type
- value
- typeof operator

> #concept boolean

- true == true
- true == 1
- true == "1"
- true == "a"
- true == "0"
- true == 0
- true == ""

> #concept comparison operators

- false === false
- "0" === 0
- "" === false

> #concept number

- Infinity
- -Infinity
- NaN === NaN
- Number constructor
  - Number('123')
  - Number('12a')
  - Number('')
- Number static
  - Number.MAX_VALUE
  - Number.isNaN(3 / window)
  - Number.isNaN(3 + window)
  - Number.isNaN(Number('x'))
  - Number.isInteger(3.1)
- funny thing about numbers
  - Number.isInteger(3 * (0.1 + 0.2) + 0.1)
  - 0.3 === 0.1 + 0.2

  > #concept Math

- Math.PI
- Math.max(1, 3)
- Math.random()
- Math.abs(-3)
- Math.sign(-3)
- Math.round(10 / 3)
- Math.ceil(10 / 3)
- Math.floor(10 / 3)
- 100 * Math.round(7.03) / 100
- Math.sqrt(10 / 3)
- Math.sin(Math.PI / 2)
- Math.cos(0)

> #concept undefined

- var a; typeof a;

> #concept string

- holds a list of characters
- str.length
- str[0]
- str.split('');
- str.toLowerCase()
- str.substring(0,1)
- str.includes('foo')
- str.indexOf('foo')



- show in [cheat-sheet](https://github.com/ironhack/bcn-webdev-cheatsheet/tree/master/m1#js-concepts)

## Code Along

> resource: [cheat-sheet boilerplate](https://github.com/ironhack/bcn-webdev-cheatsheet/tree/master/m1/)

- create folder
- create html (boilerplate)
- create js (boilerplate)
- start all files with 'use strict';

> concept: algorithm

- google algorithm

> concept: conditional
- if
- boolean expression
- if (true)

> concept: control structure
- block {}

- algorithm to log if a string contains the letter a and b

> concept: loop

- algorithm to log the first 10 [fibonacci](https://medium.com/developers-writing/fibonacci-sequence-algorithm-in-javascript-b253dc7e320e) numbers
- first as a while, refactor to a for

> concept: operator

- show in [cheat-sheet](https://github.com/ironhack/bcn-webdev-cheatsheet/tree/master/m1#js-concepts)

> mantra: code happens

- close laptops
- let's talk about time

> concept: runtime

> concept: debugging

> tool: debugger

- re-open developer tools, play with break-points + arrow down

> tool: git

- git init
- create repo
- add, status, commit, status, push, status
- activate github pages
- make them fork the repo and clone it making sure they are on their repo

## Practice

@TODO: Add link to exercice and notes