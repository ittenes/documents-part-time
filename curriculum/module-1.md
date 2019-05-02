
- http-server (when to install, when to make sure node is working)





- 2 code alongs (canvas + dom)
- 2 reference projects

- Slack Exercice part 1 + part 2





# Week 1

## Day 1

### Welcome and Orientation

### People & Stories

---
### 11:00 BREAK
---

### Deck: Class Guidelines (Irene) (15') Took 20'

### Stand-up (15')
- names and presentations

### Daily kick-off (5')
- calendar
- parking lot (example)
- feedback on feedback (example)
- feedback on calendar (example)

### Deck: Course overview (15') Took 25'

- focus on rituals
- focus on adaptive
- Deck: Cohorts

---
### 12:00 BREAK
---


### Deck: M1 (5')

- speed run everything
- going up on the wall next to the calendar
- just focus on the overview slide


### Lecture: HTML Introduction (30') - Took 30'

> #tech HTML

> #resource LU
- [LU - HTML Introduction](http://learn.ironhack.com/#/learning_unit/3015)

- Google `HTML` > wikipedia
- [The first website](http://info.cern.ch/)
- DOM tree
- html, head & body
- DOM nodes: root, ancestor, descendent, parent, child, sibling
- [element types](https://developer.mozilla.org/en-US/docs/Web/HTML/Element)
- attributes and values `src="http://..."`
- block vs inline, as in `p` vs `strong`

> #tool chrome developer tools
- the first website vs a [modern website](https://alistapart.com/)

> #resource MDN HTML
- [MDN HTML guide](https://developer.mozilla.org/en-US/docs/Learn)
- [MDN HTML reference](https://developer.mozilla.org/kab/docs/Web/HTML)

> #best Structure and content first
- google `wireframe`
- [Planning_a_simple_website](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure#Enter_HTML5_structural_elements#Planning_a_simple_website)

> #later DOM API
- manipulation
- binding/unbinding event listeners

### Quick Demo: Html Introduction (Mob website homepage, with list of students) (30')

> #resource git docs
- [git cheat-sheet](https://github.com/ironhack/bcn-webdev-cheatsheet/tree/master/tools/git)
- [git docs](https://services.github.com/on-demand/downloads/github-git-cheat-sheet.pdf)

- create repo
- clone, open in chrome
- homepage: header, section students, section resources
- page: cheat-sheet
- demo also css/js/dom but commit only the HTML

> #resource w3c validator
- [W3C HTML Validator](https://validator.w3.org/#validate_by_input)

- git demo
- deploy



---
### 13:00 LUNCH
---


### Checkpoint (10')

### Code Along: HTML Introduction (Mob website personal student page) (45')  took 1h

> #tool git

- fork
- create folder `w1/js/` and clone

> #tool vscode

- open in vscode
- open dev tools, disable cache

> #tool chrome developer tools

- add the student page HTML file (use boilerplate)
- header - h1 - your name

- test
- commit, push

> #tool github

- create pull request
- review and merge all

---
### 15:00 BREAK
---

### Lecture: JS Intro (30') Took 45'

> #tech javascript

> #resource LU
- [LU - Javascript Introduction](http://learn.ironhack.com/#/learning_unit/3012)
- [LU - Conditionals and Loops](http://learn.ironhack.com/#/learning_unit/3013)

> #concept programming

- google `programming`

> #technology javascript

- google `javascript`
- 1995 (2 years after the Internet)
- ES5 (2009) not ES6 (2015)

> #resource MDN Javascript
- [MDN Javascript guide](https://developer.mozilla.org/bm/docs/Web/JavaScript)
- [MDN Javascript reference](https://developer.mozilla.org/bm/docs/Web/JavaScript)

### Quick Demo: JS Intro (30')

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

- show in [cheat-sheet](https://github.com/ironhack/bcn-webdev-cheatsheet/tree/master/m1#js-concepts)

---
### 16:00 BREAK
---

### Code Along: JS Conditionals and Loops (HTML + JS file) (1h30')

> resource: [cheat-sheet boilerplate](https://github.com/ironhack/bcn-webdev-cheatsheet/tree/master/m1/)

- create folder
- create html (boilerplate)
- create js (boilerplate)

> concept: algorithm

- google algorithm

> concept: conditional
- if
- boolean expression

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

---
### 17:30 BREAK
---

### Lecture: Pair Programming (15')

- Google `Pair programming` wikipedia
- [Learning Unit](http://learn.ironhack.com/#/learning_unit/3018)
- [Video 2'30](https://www.youtube.com/watch?v=vgkahOzFH2Q)
- [Same Video, spanish subs](https://www.youtube.com/watch?v=T5zkEpaMlfw)
- [Talk 1:30](https://www.youtube.com/watch?v=RCDfBioUgts)

### Practice: JS basic algorithms (DE)


### Practice: HTML Introduction (Mob website student pages, profile section) (DE)
- profile section - h2, img, p, strong, em,
- interests section h3 ul li h4 ul li a

### SG: Pair Programming Introduction


## Day 2

### Review: HTML Introduction (Mob website student pages, profile section) PRs and merge (1h)

---
### 10:30 BREAK
---

### Lecture: HTML semantics & accessibility (30') Took 1h

- include `meta` to stop browser from zooming in `<head>`
- conventions
  - use double quotes around html attributes `src="http://..."`
  - IDs and classes in `class="kebab-case"`
- use outline/hierarchy:
  - h1, h2, ..., ul, li, p, strong
- use semantics:
  - nav
  - main
  - section
  - article
  - header
  - summary
  - details
  - figure
  - aside
  - figcaption
  - footer
  - mark
  - time
- use id and classes
  - e.g.: `id="site-header"`
  - e.g.: `class="card product"`
- DON'T
  - use only `<div>` and `<span>`
  - use `<br/>` unless poetry
  - add empty tags just because you need to apply some style
    - e.g.: `<div class="clear"></div>`


- [how blind navigate the internet](https://gizmodo.com/5620079/giz-explains-how-blind-people-see-the-internet)
> #tool chromevox screen reader
- [Screen Reader](https://chrome.google.com/webstore/detail/chromevox/kgejglhpjiefppelpmljglcjbhoiplfn)
- demo with https://slack.com/

- a11y
  - https://www.abrightclearweb.com/web-accessibility-in-the-uk/
  - [The a11y project][https://a11yproject.com/]
  - [WRC ARIA LAndmarks][https://www.w3.org/TR/wai-aria-practices-1.1/examples/landmarks/index.html]
  - [MDN WAI-ARIA Basics][https://developer.mozilla.org/en-US/docs/Learn/Accessibility/WAI-ARIA_basics]

> #tool tota11y accessibility test
- [Acessibility Checklist][https://a11yproject.com/checklist]
- [Tota11y](http://khan.github.io/tota11y)

> #tool no coffee vision filter
- [No Coffee](https://chrome.google.com/webstore/detail/nocoffee/jjeeggmbnhckmgdhmgdckeigabjfbddl?hl=en-GB)


### Activity: HTML diagram(s) (30')

- anatomy
  - img src
  - element type
  - attribute, value
  - p, hello **world**

- tree (teachers draw the wireframe)
  - html, head, body, header, h1, nav, main, h2, section, article, h3, img, p, link read more, another article (...) footer
  - identify root, ancestor, descendent, parent, child, sibling

- a11y
  - add `role="banner"` `role="navigation"` `role="main"`
  - add `alt="..."`

---
### 11:30 BREAK
---

### Code Along: HTML semantics & accessibility (Mob website student pages, experiments section) (30')

```html
<section class="experiments">
  <h2>Experiments</h2>
  <article class="card experiment">
    <header class="card-header">
      <h3 class="title">My first algorithm</h3>
    </header>
    <div class="card-body">
      <p><em>WIP</em>fibonacci generator</p>
      <p><a class="external" href="...">View on github</a>
    </div>
    <footer role="contentinfo" class="meta">
      <p>Created in: xx/xx/xxxx</p>
    </footer>
  </article>
</section>
```

### Review: HTML semantics & accessibility (Mob website student pages, experiments section) PRs and merge (30')

- everyone PR
- view, and merge all student pages

---
### 12:30 LUNCH
---


### Practice: Slack clone (HTML only) (1h)

- https://slack.com/

### Review: Slack clone (HTML only) PRs and comments (30')

---
### 15:00 BREAK
---

### Lecture: JS Functions and Scope (30') Took 25'

> #resource LU
- [LU - JS Functions](http://learn.ironhack.com/#/learning_unit/3020)

> #concept function

- black box metaphor (algebra function)
- name is verbSomething
- convention is camelCase
- `function addNumbers(p1, p2) { return p1 + p2 }`

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

### Quick Demo: JS Functions and Scope (30')

> #concept scope

- var num = 5;
- function addFive(p1) { var x = 1; return p1 + x + 4 }
- addFive();
- console.log(p1);

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



### Activity: role play JS debugger (30')

### Checkpoint: concepts > parking lot (10')

---
### 16:30 BREAK
---

### Lecture: JS Arrays (30')

- holds a list of values
- var arr = ['1', '2', '3'];
- var arr = new Array();
- arr.length
- arr[index]
- arr[index] = 'foo'
- arr.pop()
- arr.push('4', '5')
- arr.unshift('foo')
- arr.shift()
- arr.join(',');

```
var arr = [1332, 1232, 4332, 9873]
for var (ix = 0; ix < arr.length; ix++) {
  console.log(ix, arr[ix] / 100);
}
```

> #concept: callback (recall)

- async callback

```
console.log('before');
window.setTimeout(function () {
  console.log('1 sec later');
}, 1000);
console.log('after');
```

- sync callback

```
console.log('before');
var arr = [1, 2, 3, 4, 5];
arr.forEach(function (item, index) {
  console.log('index', index, 'item', item, 'square', item * item);
})
console.log('after');
```


### Practice: JS functions and arrays

### SG: Git Intro


## Day 3

### Review: JS functions and arrays - PRs and close (1h)

---
### 10:30 BREAK
---

### Activity: JS diagram (30')
- (statement, expression, assignment, declaration, function, parameters, return, scope, call, arguments)

### Lecture: JS Objects (30')

- holds key value pairs
- var obj = { name: 'foo' }
- obj.name = 'foo'
- obj['name-with-weird-characters'] = 'foo'
- obj[key] = 'foo'
- delete obj.name
- delete obj['name-with-weird-characters']
- delete obj[key]
- for (var key in obj) { ... }
- Object static methods
  - Object.keys(obj);
  - Object.values(obj);

---
### 11:30 BREAK
---

### Code Along: JS Codepen arrays & objects (45m)

> #concept data structure

- examples
  - https://www.nytimes.com/ (mobile)
    - list of articles with title, img (url and label), abstract, date
  - https://glovoapp.com/en/macchina-pasta-bar-2/ (mobile)
    - array of categories (sections) with different produts inside
    - https://api.glovoapp.com/v3/stores/11281/addresses/18796/collections/27278


> Tool: Codepen

- signup (with github)
- create pen
- save it as `arrays and objects`
- change layout
- open console


```js
var cohorts = [{
  city: 'bcn',
  course: 'webdev',
  date: new Date('2018-06-11'),
  name: '2018 Aug',
  students: [{name: 'Julien', country: 'es'}, {name: 'Julio', country: 'us'}]
}, {
  city: 'bcn',
  course: 'webdev',
  date: new Date('2018-08-20'),
  name: '2018 Aug',
  students: [{name: 'John', country: 'en'}, {name: 'Paquito', country: 'es'}]
}];
```

- cohorts[0].students[0].name
- for (var ix = 0; ix < cohorts length>)
- for (var ox = 0; ox < cohort[ix].sudents.length>)
- if (country === 'en') { console.log(name); }


### Review: JS Codepen arrays & objects (45m)

- embed CodePen in student page

---
### 13:00 LUNCH
---

### Practice: JS clue (1h)

### Review: JS clue - PRs and close (30')

---
### 15:30 BREAK
---

### Lecture: CSS Intro (anatomy, reset, box model) (30')

- rule
- selector
- declaration: property, value
- shorthand property
- specifity
- pseudo-selector
- https://cssreference.io/
- and more:
- user agent styles
- reset
- box model

- width, padding, margin
- when not floated or `position:absolute` or `position:fixed` every block element is naturally `100% wide`
- 100% of what!?

> #resource MDN CSS
- [MDN CSS guide](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS)
- [MDN CSS reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input)

### Code Along: CSS layout: fluid, float, clear (30')

- teacher on the homepage
  - add a footer with floated elements
  - 50%, 50% + padding does not fit!!!

- students on their page
  - add the html
  - add the box-model reset
  - still doesn't fit
  - add the body reset

> #best simplicity

- fluid container, margin-bottom, padding-top
- float, clear and overflow

> #mantra kiss

> #concept positioning
  - [demo](http://www.webdevbydoing.com/whats-the-difference-between-static-relative-absolute-and-fixed-positioning/)
  - `position: relative`
    - used with `top/left` displaces the element (but the original space is still occupied)
    - establishes an anchor for absoulte descendent
  - `position: absolute`
    - element complete leaves the flow
    - and looses its natural block ability of being `width 100%`
    - used with `top/left`, always relative to first `absolute` OR `relative` ancestor
  - `position: absolute`
    - used with `top/left` always relative to `body`

---
### 16:30
---

### Lecture: CSS Styling (typography, color, links and buttons) (30')

- DRY
  - use hierarchy
    - `<div class="card"><div class="title">...`
    - target via `.card .title {}`
  - use composition
    - combine classes
    - `class="button primary"` targeted via `.button.primary {}`
  - use cascading
    - specifics augment and override generics
    - `#login-button` stronger than`.button {}` stronger than `a {}`
  - use inheritance
    - type attributes (font-family, font-size, line-height, color, ...) trickle down from parent to children
- semantic:
  - semantic css, classes named after what things ARE not what they LOOK LIKE
    - e.g.: `.copy`, `.site-header`, `.copyright`, `.email` ...
- short selectors
  - e.g.: `.header li`

---
### 17:00 BREAK
---

### Code Along: CSS Codepen typography and color (30')

- [Google Fonts](https://fonts.google.com/)
- body , h1, h3, p, strong
- [Colorzilla](http://www.colorzilla.com/chrome/)
- [Colors](https://coolors.co/)
- [Colors](http://paletton.com/)

- USE INHERITANCE: body font, card font

- USE HIERARCHY: `.card .title

### Code Along: CSS Codepen links and buttons (30')

- a .button .primary .secondary
- USE COMPOSITION `.button.primary`

--/--

### Practice: Slack clone (CSS layout and styling) (DE)

### SG: CodeWars


## Day 4

### Review: Slack clone (CSS positioning and styling) PR and comments (1h)

---
### 10:30 BREAK
---

### Practice: Slack clone (30')

### Lecture: CSS Responsive Web Design (30') Took 20'

- [responsive web design](https://en.wikipedia.org/wiki/Responsive_web_design)
- how the paradigm shifted from desktop first to mobile first
  - right after it changed from graceful degradation to progressive enhancement
- small/big apartment metaphor
- [9 basic principles](http://blog.froont.com/9-basic-principles-of-responsive-web-design/)
- content is like water mantra
- explain the use of max-width
- [search responsive on css-tricks](https://css-tricks.com/?s=responsive+&orderby=relevance&post_type=post%2Cpage%2Cguide)
- [responsive design](https://alistapart.com/topic/responsive-design)

### Quick Demo: CSS Responsive Web Design (Mob Website main page)

- add css file with boilerplate
- add classes included in the boilerplate to the site
- make divs inside the container to contain the content but not the background color
- show the container not growing past 768px (media query included)
- show why the media query has max-width 728 (original container margin)
- float the two lists side by side

### Activity: CSS diagram (including media query) (30')

- rule, selector, class, pseudo-class, property, value, shorthand property. shorthand value, unit, color

```css
.card:hover {
  border: 1px solid black;
}
@media (min-width: 728px) {
  .card {
    background-color: #efefef;
  }
}
```

---
### 11:30 BREAK
---

### Lecture: CSS Flexbox (30')

- [flexbox CSS Tricks Guide](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)
- [flexbox froggy](https://flexboxfroggy.com/)
- draw on the board a wire frame and sample html and explain the approach with float (try to match the colors)
  - html - header>img+nav>a*2
- convert the rules to flexbox on the board
- explain the rules that apply to the parent
- [flexbox MDN](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout/Basic_Concepts_of_Flexbox)
- use the examples to play with the boxes
- explain the rules that apply to the children

### Code Along: CSS Flexbox (Mob website CSS homepage + student pages) (1h)
- add the header/footer and container to all pages
- stretch goal style profile section
- stretch goal style experiments section

---
### 13:00 LUNCH
---

### Practice: Slack clone (CSS responsive) (1h)

WARNING: risk of running out of time/steam
/ consider pushing to the next day and stay on CSS
/ + Lecture: CSS Forms
/ + Practice:  practice exercise @todo Mob website vs codepens

### Review: Slack clone (CSS responsive) PRs and close (30')

---
### 15:30 BREAK
---


### Lecture: JS Arrays - Map, Reduce, Filter and Find (30')

> array methods

- arr.find( callback )
- arr.map( callback )
- arr.reduce( callback )
- arr.filter( callback )

### Activity: role play card deck arrays (conversation between method & callback) (30')

---
### 16:30 BREAK
---

### Lecture: JS Arrays - Sort, Reverse & Splice  (30')

> array methods

- arr.sort( callback )
- arr.reverse()
- arr.splice(1, 2)
- arr.splice(1, 0, 'foo')
- arr.slice(1, 2)

### Activity: array function diagrams (30')

Make the examples close to reality. (E.g. people, scores, etc)

- find
- filter
- map
- reduce

### Activity: role play bubble sort (30')

- age/name
- start with one a/b pass one by one (the teacher asks)
- let them rearrange themselves for a while
- interrupt when it's almost done
- finish with an a/b pass to correct/confirm

### Practice: JS all times movies (DE)

### SG: CodeWars






## Day 5

### Review: JS all times movies PRs (1h)

---
### 10:30 BREAK
---

### Lecture: DOM Introduction & Selectors (30')

- window.document
- window.onload = function () { ... }
- document.body
- node = document.getElementById('site-header')
- node = document.getElementsByClassName('feature')
- node = document.querySelector('.features .feature')
- nodeList = document.querySelectorAll('.features .feature')

- half quick/demo
- show in slack.com

```js
var img = document.querySelector('.o-hero img');
img.setAttribute('src', 'https://pbs.twimg.com/profile_images/844137908252610566/OsT9RU83_400x400.jpg');
img.removeAttribute('srcset');
```
- node.setAttribute('src', 'https://fakeimage.com/image.jpg')

- node.removeAttribute('srcset');

- node.classList.add('active') node.classList.remove('active')

- node.classList.toggle('active')

- node.appendChild(child)

- node.children[0]...

- node.remove()

- ole=search input

  input change

  event handler

  show box with results

  empty results

  results = students.filter

  add dom with students

  or "no students match foo"node = document.createElement('div')

- node.innerHTML = `'<p>some text</p>'`

- node.innerText = 'some text'

#### Lesson Notes

- refresh what is the DOM, explain the why and the possibilities
- explain what is window and document
- open a random page like github and select elements demoing querySelector & querySelectorAll
- explain the older selection APIs like getElementById & getElementsByClassName
- show how you can find the parents & siblings of a selected element
- on the main page of the mob website
  - show how to add a new section creating a section element
  - create an h2
  - add text to the h2
  - append the h2 to the section
  - append the section to the website before the footer
- make sure you show that as long as you have the variable with the element, you have control, even if the element is removed from the DOM, it can be added again

### Lecture: DOM Manipulation & Events (30')

- node.addEventListener('click', handleClick);
- node.removeEventListener('click', handleClick);
- function handleClick(event) { ... }
- event.stopPropagation();
- event.preventDefault();

- half quick/demo
- show in slack.com

```js
var button = document.querySelector('a.v--secondary');
button.addEventListener('click', function (ev) {
  ev.preventDefault();
  button.parentElement.parentElement.classList.add('is-hidden');
});
```
- event.target
- event.currentTarget

```js
var ps = document.querySelectorAll('p');
for (var ix = 0; ix < ps.length; ix++) {
  ps[ix].addEventListener('click', function (ev) {
    ev.preventDefault();
    ev.currentTarget.style.color = 'red';
  });
}
```

#### Lesson Notes

- on the main page of the mob website
- show how to select both h2 titles
- loop through them and add an event listener to each one of them with an anonymous function
- inside of the function, show them how to select the ul's of both sections by going up to the parent and then selecting the ul inside of it
- toggle the class hidden to the ul that you want to show and hide

```javascript
'use strict';

function main() {
  var nodes = document.querySelectorAll('section h2');

  for (var ix = 0; ix < nodes.length; ix++) {
    nodes[ix].addEventListener('click', function (event) {
      var h2 = event.currentTarget;
      var section = h2.parentNode;
      section.classList.toggle('expanded');
    });
  };
}

window.addEventListener('load', main);
```



---
### 11:30 BREAK
---

### Quick Demo: DOM Manipulation & Events (Mob website homepage, search students) (30') Took 1h45'

- `var students` in a file everyone can load with script src
- form role=search input
- input change
- event handler
  - show box with results
  - empty results
  - results = students.filter
  - add dom with students
  - or "no students match `foo`"

#### Quick Demo Notes

- add the ironhack remote to everyone
  - `git remote -v` to check if the remote is added already
  - `git status` to check if there are changes (if yes, add, commit, push and PR)
  - `git remote add ironhack https://github.com/ironhack/<remote-url>` to add the ironhack remote
  - `git pull ironhack master` to pull the changes from ironhack
- explain (draw) on the board what is going to happen
  - add an input to a new sub header that will search and filter the array
  - it will display the list on an absolute positioned list
- add the array with students.js in the main folder
- explain the steps until they are able to console.log the input value and give them 5 minutes to achieve it
- allow everyone to reach that and explain the next step on the board.
  - store the input value on a variable
  - filter the results of the array
  - console.log the result
- append each one of the results as an  `a` tag to the DOM, make sure the link works
- re-factor the code and explain the importance of it
- build the list with an `ul`. appending the `a` to the `li`, the `li` to the `ul` and finally the `ul` to the search results
- style the results div with absolute positioning so that it appears right below the search box

---
### 12:00 LUNCH
---

### Practice: DOM Manipulation & Events (Mob website homepage, search students) (1h30')

- allow students to organise mobs
- students add a box to search

### Review: DOM Manipulation & Events (Mob website homepage, search students) (30')

---
### 15:00 BREAK
---

### Lecture: JS Object Oriented Intro AND JS Prototypal inheritance (1h)

 - The basic idea of OOP is that we use objects to model real world things that we want to represent inside our programs, and/or provide a simple way to access functionality that would otherwise be hard or impossible to make use of.
 - Objects can contain related data and code, which represent information about the thing you are trying to model, and functionality or behavior that you want it to have. Object data (and often, functions too) can be stored neatly (the official word is **encapsulated**) inside an object package 

---
### 16:00 BREAK
---

### Lecture: Talk `Backstory of WebDev`

- [slide deck](https://docs.google.com/presentation/d/1jWWXcb6mbLpmyNICQq9qWyNQq3syvrGhjji-72h01Bo/edit#slide=id.g3a834f7172_0_0)


### Practice: JS vikings (DE suggest pairing / mobbing) (DE)
### Practice: Mob website (DOM student pages - show/hide experiment sections) (DE)
### Practice: Mob website (DOM student pages - add list of students to DOM from array) (DE)[]()

### Lecture: Events

- ev.stopPropagation()
- ev.preventDefault()
- explain how event propagation  works in the board, drawing a small tree of elements and ask if an event will 'move up' the DOM tree.
- explain what happens when two different events happen, one in body and one in main
  - which one goes first
  - explain with a narrative, introduce the word propagate and event propagation
- on the mob website, add an event on body and another on the input of the student search, code the stopPropagation()

#### Practice: Events

- challenges for students to practice
  1. hide the search results when
     1. click on body (requires to stop propagation when click on input)
     2. press esc
  2. show the results again when
     1. input focus

### Lecture: Async

 - Show the 4 native functions, and explain that setInterval and setTimeout return a number (an id)
    - setTimeout(function () {}, 1000)
    - setInterval(function () {}, 1000)
    - clearInterval(intervalID)
 - do small 30 second counter using the setInterval and clearInterval
 - give an example of when you should use a clearTimeout



#### Practice: Async

- challenges
  - counter for 30s on the top corner (setTimeout)
  - need to click a hidden work/object on the page to cancel the timer (clearInterval)



### Code Along: HTML+CSS Game (took 6h)

- do an up or down type of game where you try to guess if the next number is bigger or smaller than the next
  - example repo: https://github.com/tawebbcn/up-or-down
- do small steps and try to make sure that everyone is able to keep up
- if too lost, then ask to continue later
- start with main.js, building up the flow between the three screens



### Code Along: Canvas Game

- do planing on the board and write the data structures and wireframe
- try to adapt the code from the previous code along if possible
- clean up the dom elements used to do the game
- build the new dom with the lives, score and canvas elements
- if you want to go responsive, make the div around the canvas flex:1 and inside of the game.js read the offsetHeight/offsetWidth and apply them to the canvas


### Lecture: SASS

#### advantages:
- maintainability
- DRY (nesting, variables)
- small files
- easier to read (@import)
- allows use of other people’s code 
- you don’t need to load the whole CSS file, just the part that you want/need

two ways to write:
- scss(with { })
- sass(with tabs)

#### summary:

- it’s a language and a tool that transforms scss code into css

- best practices are key

- you can and should nest instead of advanced selectors; it will compile to normal css

- you can nest classes and also properties (eg: background-xxx)

- you can create variables (with the dollar sign $) and can reuse them throughout your code (useful for color and padding)

- use "&" to nest

- @import allow you to import small parts of other people's code

- @extend allow you to reuse parts of the code. It extends the rules of another class/variable

- @include is exactly like the extend except what you're including is not a css selector ( you have to define the @mixin before)

- @mixin behaves like a function. it can receive arguments and it runs the code where it is called (arguments can have defaults in case you want to call it without giving the arguments)

- sass warns you about erros in your code and refuses to compile it

#### best practices:

- best practice is to have two files (one with your variables and one with your mixins)

- don't nest too deep

- use @mixin all the time

- never commit your css files to your repository unless you need to (add it to .gitignore)

#### tool installing:
 - node-sass
 - it's the fastest tool for js
 - npm install -g node-sass

#### practicing:
- changed the files of the game code-along to train with the new tool

#### compiling
- node-sass --output-style compressed --source-map true --watch style.scss style.css

#### steps taken:
- little intro
- summary of scss features (all kinds of nesting, variables and mixin)
- best practices (do's and dont's)
- install tool to compile
- practice



## Parking Lot

### Lecture JS | Async & Callbacks (30')

### Practice: JS timer (1h30)

### Quick Demo: HTML Game Interaction (1h)

### Quick Demo: Canvas Intro + Basic Drawing (1h)

### Long Demo: HTML Game (2h)

### Long Demo: Canvas Game (2h)

### Project Kick-off

### Project: Planning Session

### Lecture: Kanban

### Code Along: Game Design (2h)

### Code Along: HTML+CSS Game

### Code Along: Canvas Game

### SG: Markdown and READMEs



# Adaptive

## Agile

### SG: Project Management

### Talk: `agile 101`
- [slide deck](https://docs.google.com/presentation/d/1IWIH8DSQuwssG1NIzi2oFaFjCDf_nrvhI7uS6y8Q3w8/edit#slide=id.g3a6b345037_0_152)


## HTML

### Practice: HTML (Glovo clone - html only)


## DOM

### DOM Codepen: search box (countries, songs, ....)
### DOM/JS Codepen: manipulation with constructors `var a = new Thing(data) - appendChild(thing.getDom())`


## CSS

### Practice: CSS styling (Glovo clone - container, typography, color, links and buttons)
### Practice: CSS (Glovo clone - flexbox, responsive)
### Practice: CSS (Glovo clone - transitions)
### Practice: DOM (Glovo clone - burger menu)
### [Advanced] Quick Demo: Transitions & Animations
### [Advanced] CSS Codepen: display label with animation when field is focused https://codepen.io/SitePoint/pen/zGyLt
### [Advanced] Lecture: Styleguide Driven Development
### [Advanced] Code Along: Styleguide Driven Development


## Bootstrap

### Lecture: Bootstrap Intro + Components

## JQuery

### Quick Demo: jQuery manipulation + events
### Lecture: jQuery Introduction, DOM Selectors + Events
### Code Along: jQuery manipulation + traversing
### Codepen: jQuery manipulation
### [Advanced] Quick Demo: jQuery Animations


## Build

### [Advanced] Lecture: build, minification, uglification
### [Advanced] Code Along: webpack + livereload


## Advanced JS

### [Advanced] Lecture: JS Function + Context
### [Advanced] Lecture: JS Closures + Scope
### [Advanced] Lecture: JS Functional programming, higher order functions
### [Advanced] Lecture: JS Testing + Jasmine
### [Advanced] Practice: JS Advanced algorithms

### [Advanced] Quick Demo: PWA


## Libraries

### [Advanced] Quick Demo: JS Lodash Intro
### [Advanced] Quick Demo: Moment.js


