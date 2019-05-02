# DOM Intro & Selectors

## Lecture notes

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