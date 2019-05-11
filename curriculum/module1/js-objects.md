# JS Objects

## Lecture Notes

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

## Code Along: JS Codepen arrays & objects

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


## Practice

- Code Pen: https://codepen.io/tawebbcn/pen/dggwBJ
- Code Pen 2: https://codepen.io/tawebbcn/pen/eLbppm
- JS Clue 

@Todo, link and notes