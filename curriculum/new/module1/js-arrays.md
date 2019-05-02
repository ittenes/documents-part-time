# JS Arrays

## Lecture

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

## Practice

- JS functions and arrays
  link: https://github.com/Ironhack-PartTime-BCN/bcn-webdev-checklists/blob/master/labs/m1/lab-javascript-functions-and-arrays.md
  
@Todo, add notes to the exercice
