# Week 1 - Day 2 (Thursday)

## HTML

- What is HTML
- DOM Tree
- Tags
- Block vs Inline
- Semantic Tags

- [https://devhints.io/html](https://devhints.io/html)

## CSS

- What is CSS
- Specificity
- inline Style
- styles in head
- styles in file

- Selectors (.class #id tag)
- BEM (Block Element Modifier)

- Box Model

  - margin
  - border
  - padding
  - box-sizing

- Positioning

  - static
  - relative
  - fixed
  - absolute
  - Floats
  - Clear Floats

- Reset
- Structure

  - Layouts, Typography ...

- [https://devhints.io/css](https://devhints.io/css)
- [CanIUse]()

## Git

- git status
- stage
- git add
- git commit
- git checkout
- git branch
- github

# Week 1 - Day 3 (Saturday)

## JS

- What is JS
- concepts assignment statement expression
- types of variables
  - bool
  - number
  - string
  - func
  - array
  - object
  - null
  - undefined
- types of Variables
  - var
  - let
  - const
- naming variables [Link](http://bensmith.io/20-tips-for-better-naming) - [Link](https://hackernoon.com/the-art-of-naming-variables-52f44de00aad)
  - verbs -> func
  - answerYesNo -> bools
  - arrays in plural
- Operators
  - PEMDAS
- Methods Number / String
  - slice
  - substring
  - repeat
  - indexOf
- Boolean Operators
  - AND
  - OR
  - NOT
- Conditional and Loops

  - if
  - if else
  - if else if
  - switch
  - for
  - while
  - do while
  - forEach

- Inmutabilidad

- Functions
  - named
  - anonymous
- Arrays
  - methods

# Week 2 - Day 1 (Tuesday)

- CSS Advanced Selectors [Link](https://devhints.io/css)
  - Descendants
    - Direct Descendants
    - Descendants Selectors
  - Siblinds
    - Adjancent
  - Multiple selections
  - Attribute selectors
  - Pseudo-Classes

# Week 2 - Day 2 (Thursday)

- Objects
- Arrays
- Mutability in Objects and Arrays

# Week 2 - Day 3 (Saturday)

- Array Methods

  - Map
  - Filter
  - Splice
  - Reduce
  - Sort

- OOP

# Week 3 - Day 1 (Tuesday)

- Responsive Design
- Flexbox
- 12 Columns

# Week 3 - Day 2 (Thursday)

- DOM Manipulation
- window.document
- window.onload = function () { ... }
- document.body
- node = document.getElementById('site-header')
- node = document.getElementsByClassName('feature')
- node = document.querySelector('.features .feature')
- nodeList = document.querySelectorAll('.features .feature')
- show in slack.com

```js
var img = document.querySelector(".o-hero img");
img.setAttribute(
  "src",
  "https://pbs.twimg.com/profile_images/844137908252610566/OsT9RU83_400x400.jpg"
);
img.removeAttribute("srcset");
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
  [Link](https://gist.github.com/thegitfather/9c9f1a927cd57df14a59c268f118ce86#accessing-dom-elements)
- node.addEventListener('click', handleClick);
- node.removeEventListener('click', handleClick);
- function handleClick(event) { ... }
- event.stopPropagation();
- event.preventDefault();

- half quick/demo
- show in slack.com

```js
var button = document.querySelector("a.v--secondary");
button.addEventListener("click", function(ev) {
  ev.preventDefault();
  button.parentElement.parentElement.classList.add("is-hidden");
});
```

- event.target
- event.currentTarget

```js
var ps = document.querySelectorAll("p");
for (var ix = 0; ix < ps.length; ix++) {
  ps[ix].addEventListener("click", function(ev) {
    ev.preventDefault();
    ev.currentTarget.style.color = "red";
  });
}
```
