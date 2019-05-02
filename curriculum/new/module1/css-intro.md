# CSS Intro

## Lecture Notes

- rule
- selector
- simple selectors
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

- [Best Practices](https://github.com/ironhack/bcn-webdev-cheatsheet/tree/master/m1#css-best-practices)

> #resource MDN CSS
- [MDN CSS guide](https://developer.mozilla.org/en-US/docs/Learn/CSS/Introduction_to_CSS)
- [MDN CSS reference](https://developer.mozilla.org/en-US/docs/Web/CSS)
- [W3C CSS Validator](https://jigsaw.w3.org/css-validator/#validate_by_input)


## Code Along

- https://codepen.io/tawebbcn/pen/ZqRdvz (https://codepen.io/tawebbcn/pen/ZqRdvz)
- http://jsfiddle.net/Mvv8w/4/ (Overflow hidden fix)
- https://codepen.io/tawebbcn/pen/QZxebL (container example)
- https://codepen.io/tawebbcn/pen/pOqGod (position)

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

## Activity

### CSS Diagram

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