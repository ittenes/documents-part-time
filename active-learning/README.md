# Active Learning

## You do it
- [Mini Projects](./mini-projects.md)
- [Code Along](./code-along.md)
- [Project Review](./project-review.md)

## Watch and learn
- [Quick Demo](./quick-demo.md)

## You be it (role plays)

- Be the app.js (understand flow and importance of order of middlewares)
  - one person is one middleware (e.g. static)
  - one person is anotehr middleware (e.g. body parser)
  - one person is a route controller (e.g. POST /foobar - validate body)
  - another one for is the 404 middleware
  - one is express, creates a res object, passes it to middlwares, receives it back (next!)
  - one person is http, taking requests from the user to express and the response back
  - teacher is the user, send requests

- Be the callback of array sort, array filter, array find and array reduce
  - the array is deck with 5 cards
  - let's e.g. `sort by suit, then color (red first)` or `filter out reds` or `map to `
  - one person is the callback
    - receives the params (the card, the acc on a post-it/whiteboard, ...)
    - and should return according to input and the purpose
  - another person is the array.fn implementation
    - calls the callback person (gives card, writes acc+item+index on whiteboard)
    - prepares the resulting array according to the callback return value
  - easiest way to start is teacher is the `array.fn` and one student is the callback

- Be the element of a bubble sorte by name / age
  - show them the hungarian dancers
  - everyone against the wall
  - bubble sort yourselves by name/age (let chaos ensue)
  - do a final pass, one by one and out loud, to check sorting worked (helps people know each other)

- Be the JS interpreter (functions, variables, scopes)

## You explain it

- Go in front of the class and explain the flow that is written/drawn on the board

## You draw it
- MODULE 1
  - HTML structure
  - Basic Javascript definitions and names
  - Basic CSS rules
  - A DOM event+manipulation example
  - constructors and instances
  - how to structure different kinds of games

- MODULE 2
  - ES6 changes
  - HTTP workflow
  - Express req/res (with 1 middleware + route > mongoose + 404, no 3rd party APIs)

- MODULE 3
  - Angular component hierarchy and I/O flow

## Others
- Groups for the day
- Mobbing a PP exercise (max per group 7, requires one projector per group)

