# HTML Intro

## Lecture

- Check everyone with Windows 
- Check everyone with VS Code

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
- self-closing tags
- double-quotes always
- kebab-case

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

## Quick Demo

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

## Code Along

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

## Practice

- (Mob website student pages, profile section) PRs and merge (1h)
- profile section - h2, img, p, strong, em,
- interests section h3 ul li h4 ul li a

## Review

@TODO - Minimum standards for the PR

## Activity

- anatomy
  - element type, attribute, value, block, inline
```html
  - <p>my photo <img src="..." alt="me and my dog" /></p>
```

- tree (teachers draw the wireframe)
  - html, head, body, header, h1, nav, main, h2, section, article, h3, img, p, link read more, another article (...) footer
  - identify root, ancestor, descendent, parent, child, sibling

- a11y
  - add `role="banner"` `role="navigation"` `role="main"`
  - add `alt="..."`