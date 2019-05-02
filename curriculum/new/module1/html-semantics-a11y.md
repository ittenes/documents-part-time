# HTML Semantics & Accessibility

## Lecture Notes

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


## Code Along

- @Todo - purpose and steps to explain
- can be used to introduce emmet

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

## Practice

- Clone Slack part 1
- Mobile first
- Warn about A/B testing
- Skip one section