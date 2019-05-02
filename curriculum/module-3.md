# Module 3

# Week 7

## Day 1

### 9.30 Retrospective
  - [Retro - checklist](https://github.com/ironhack/webdev-checklists/tree/master/retrospectives)

---
### 11.30 Break
--- 

### Research: Typescript & dynamic vs static types
  - typescript
  - dynamic typed vs static typed languages

### Research review: Typescript & dynamic vs static types

---
### 13.00 Lunch
--- 

### Lecture: Typescript (30min)
  - introduccion
    - created by microsoft
    - open source
    - superset of javascript
    - static typing
    - modules, namespaces and strong OOP support
    - compilation step (catch errors)
  - installation
    - `npm install -g typescript`
    - type `tsc` in the terminal to check installation
  - compilation
    - type `tsc name-of-the-file.ts` to compile
    - file extension .ts > .js
  - features
    - types
      - file extension .ts > .js
      - `let myVarName: dataType = value;`
      - `let myNumber:   number  = 42;`
        `let myBoolean:  boolean = true;`
        `let myString:   string  = "Hello World";`
        `let unusable:   void    = undefined; // Used for functions which don't return a value.`
        `let myWhatever: any     = { hello: 'World' }; // Can be any other type`
    - generics
      - JavaScript arrays are an example of a generic type because they can hold elements of any type
      - `let myArray: Array<T> = [];`
      - `let myArray: Array<string> = ['a','b','c']; // Array of strings`
      - `let myArray: Array<number> = [1, 2, 3]; // Array of numbers`
    - interfaces
      - are like an abstract class (you cannot create objects out of an interface, classes can implement an interface)
    - classes
    - decorators
      - A Decorator is an object-oriented pattern that adds behaviour to classes and methods
      - A decorator is just a function that is going to decorate (populate) a target.

  - resources
    - [TypeScript - JavaScript that scales.](https://www.typescriptlang.org)
    - [What is TypeScript and why would I use it in place of JavaScript? - Stack Overflow](https://stackoverflow.com/questions/12694530/what-is-typescript-and-why-would-i-use-it-in-place-of-javascript/35048303#35048303)

---
### 14.30 Break
---

### Lecture: Hello Angular 2 (1h)
  - client-server arquitecture
  - backend rendered vs frontend rendered
  - SPA (single page applications)
  - Angularjs vs Angular 2+
  - resources:
    - [Angular Docs](https://angular.io/)

---
### 15.40 Break
---

### Quick demo: Mob website from BE render to FE render (2h 15min)
  - mob website
    - we will expose events (response as json)
    - create an angular app to render events in the frontend
  - thing to show during the live code:
    - backend setup (postman)
    - app initialization
    - tipical angular arquitecture
    - how to initialize services, pages and components
    - modules
    - event service & httpClient
    - dependency injection
    - components
    - ngIf (loading pattern), ngFor (list of cards)

### Practice: Typescript
  - as we dont give today the component lecture they are wont be able to do the angular daily, an option is to give the typescript PP exercise as daily
  - [GitHub - ironhack-labs/lab-typescript](https://github.com/ironhack-labs/lab-typescript)

### Research: SPA frameworks (history) & RestAPI
  - SPA frameworks (history)
  - RestAPI
  
## Day 2

### Review: SPA frameworks (history) & RestAPI

### Lecture: Angular components (2hs)
  - install CLI `npm install -g @angular/cli`
  - ng new, ng generate & ng serve
  - tipical angular arquitecture (building blocks)
    - components & pages
    - services
    - pipes
  - components introduction:
    - life cycle hooks (constructor, ngOnInit, ngOnchanges, ngOnDestroy)
    - component structure (encapsulated MVC)
    - how to render a component on a template
    - nested components

---
### 11.30 Break
---

### Lecture: Angular modules and ngModule (1h 20min)
  - modules in ESM
    - module declaration (with export)
    - module import
  - ngModule
    - explain how modules work in angular
    - how to import a ngModule
    - appModule

---
### 13.00 Lunch
---

### Lecture: Angular data binding (1hs 40min)
  - interpolation `{{}}`
  - property binding `[]` (data flow from logic layer to the template)
  - event binding `()` (data flow from template to logic layer)
  - to ways data binding `[()]` (data flow in the two ways) (requires forms module)
  - template variables `#`

---
### 15.40 Break
---

### Activity: Components (40min)
  - MVC with the 3 parts of the components
  - explain in the templates {{}}, [], (), [()]

### Review: Group activity (30min)

### Lecture: Angular directives (1h)
  - what are directives
  - ngIf (to display or hide)
  - ngFor (to iterate)
  - ngSwitch (when you have several case for many conditions)
  - ngClass (to dynamically apply css classes)
  - ngStyle (to set css property to an element)

### Research: Services & Ajax in angular

### Practide: Ironcontacts
  - [GitHub - ironhack-labs/lab-ironcontacts](https://github.com/ironhack-labs/lab-ironacontacts)


## Day 3 

### Review: Services & Ajax in angular (30min)

### Slow demo day
  - all day combining research + demo + mobbing with the students (dont try this at home)
  - same backend
  - api route
  - instagram clone (images)

### Quick demo: Services (1h 30min)
  - why we use services
    - dry / abstraction (talking to API)
    - sharing state between components
  - using services
  - service injection
  - multiple instance vs singleton
  - dependecy injection
  - httpClient

---
### 11.30 Break
---

### Quick demo: Routing (1h 50min)
  - angular router
  - setting up routes
  - router outlet
  - RouterLink
  - route parameters
  - router navigate

---
### 13.00 Lunch
---

### Quick demo: Rest API Express (1h 50min)
  - REST Overview
  - Setup an API (express)
  - http mehods
  - postman
  - CORS!!!!

---
### 16.00 Break
---

### Quick demo: HTTP (1h 30min) 
  - HttpModule
  - http in services
  - observables in http
  - we use promises

### Practice: Cinema billboard
  - find other exercise
  - [GitHub - ironhack-labs/lab-angular-cinema-billboard](https://github.com/ironhack-labs/lab-angular-cinema-billboard)

## Day 4

### Activity: RestAPI (Planning) (30min)
  - planning
  - setting up server
  - setting up models
  - setting up routes
  - test routes in postman

### Activity: RestAPI (Mob programming) (3hs)

---
### 13.00 Lunch
---

### Activity: SPA Frontend (Planning) (30min)
  - setting up client
  - generate components
  - generate services

### Activity: SPA (Mob programming) (3hs)

### Practice: Weekend
  - add api route to the mob website backend
  - Mob website mobile apps

### Research: Pipes
  - Add a date pipe in the daily exercise

## Day 5 (Tunathon)

## Parking lot

## Day 1 (week 2)

### Lecture: Forms (1h 30min)
  - forms module
  - input validation

### Lecture: Component I/O (1h 30min) (11.10 to 12.30)
  - component interaction
  - input
  - output
  - 
### Activity: Components I/O (30min) (12.30 to 13.00)
  - `app-card [item] (delete)`
  - 
### Lecture: Authentication (2hs) (9.30 to 11.30)
  - setting up the backend
  - test in postman
  - setting up the client
    - components nedded
    - auth service

### Break (15min) (11.30 to 11.45)

### Lecture: Route guards (1h 15min) (11.45 to 13.00)
  - canActivate
  - canDeactivate

### Project kickoff (1h 15min) (11.45 to 13.00)

### Lecture: Deployment
### Lecture: File upload
### Lecture: Maps
