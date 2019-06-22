# Easy Katas Modulo 1

- [Number of anagrams in an array of words: ](https://www.codewars.com/kata/587e18b97a25e865530000d8)
```
function anagramCounter (wordsArray) {
  let counter = 0;
  wordsArray.forEach((string, index) => {
    for (let i=(index+1); i < wordsArray.length; i++) {
      if (string.length === wordsArray[i].length){
        (wordsArray[i].split("").filter(letter => string.includes(letter)).length === string.length) && counter++;
      }
    }
  });

  return counter;
}
```

- [Sum Mixed Array: ](https://www.codewars.com/kata/57eaeb9578748ff92a000009)
```
function sumMix(x){
  return x.reduce((total, n) => total += parseInt(n), 0)
}
```

- [Count of positives / sum of negatives: ](https://www.codewars.com/kata/576bb71bbbcf0951d5000044)
```
function countPositivesSumNegatives(input) {
    let result = [];
    let counter=0;
    let accumulator = 0;
    
    if ( input && input.length >= 1){
      input.forEach(num => {
        if (num > 0){
          counter++;
        } else {
          accumulator += num;
        }
      });
      result[0]= counter;
      result[1]= accumulator;
    }
    
    return result;
}
```

- [Get the mean of an array](https://www.codewars.com/kata/563e320cee5dddcf77000158)
```
function getAverage(marks){
 return Math.floor(marks.reduce((acc, curr) => acc + curr, 0) / marks.length)
}
```

- [Find numbers which are divisible by given number](https://www.codewars.com/kata/55edaba99da3a9c84000003b)
```
function getAverage(marks){
  return parseInt((marks.reduce((total,n) => total+=n,0)) / marks.length);
}
```


- [Remove First and Last Character](https://www.codewars.com/kata/56bc28ad5bdaeb48760009b0)
```
function removeChar(str){
  return str.slice(1, str.length-1);
};
```

- [List Filtering](https://www.codewars.com/kata/list-filtering/javascript)

```
function filter_list(l) {
  return l.filter(item => typeof item === 'number')
}
```

- [Sum of all the multiples of 3 or 5](https://www.codewars.com/kata/sum-of-all-the-multiples-of-3-or-5/javascript)

```
function findSum(n) {
  let sum = 0;
  for (let i = 0; i <= n; i++) {
    if (i % 3 === 0 || i % 5 === 0) {
      sum += i;
    }
  }
  return sum;
}
```

- [Vowel Count](https://www.codewars.com/kata/vowel-count)

```
function getCount(str) {
  return str.split('').filter(letter => 'aeiou'.includes(letter)).length
}
```

- [Flatten](https://www.codewars.com/kata/flatten-1/javascript)

```
var flatten = function (array){
  return [].concat.apply([],array)
}
```

# Easy Katas Modulo 2

- [Square Every Digit](https://www.codewars.com/kata/square-every-digit/train/javascript)

```
function squareDigits(num){
  return Number([...num+ ''].map(number=>number**2).join(''))
}
```

- [Credit Card Mask](https://www.codewars.com/kata/credit-card-mask/train/javascript)

```
function maskify(cc) {
   return cc.slice(0,-4).split('').map(number => number = '#').join('')+`${cc.slice(-4)}`

}

```

- [Find the odd int](https://www.codewars.com/kata/find-the-odd-int/train/javascript)

```
function findOdd(A) {
  let result=[];
  A.forEach(number => {A.filter(v => v === number).length % 2 !== 0 && result.push(number)})
  return result[0]
}
```

- [Jaden Casing Strings](https://www.codewars.com/kata/jaden-casing-strings/train/javascript)

```
String.prototype.toJadenCase = function () {
return this.split(' ').map(word => word.charAt(0).toUpperCase() + word.slice(1)).join(' ')
};

```

# Easy Katas

- [Drone Fly By](https://www.codewars.com/kata/drone-fly-by)

```
const flyBy = (lamps, drone) => [...lamps].fill(`o`, 0, drone.length).join(``)
```

- [Growth of a population](https://www.codewars.com/kata/growth-of-a-population)

```
function nbYear(p0, percent, aug, p) {
    // your code
    if (p0 >= p) {
      return 0;
    }

    return 1 + nbYear(p0 + p0 * percent / 100 + aug, percent, aug, p);
}
```

- [Inverting a Hash](https://www.codewars.com/kata/inverting-a-hash/javascript)

```
function invertHash(hash) {
  inverted = {};

  for (const [key, value] of Object.entries(hash)) {
    inverted[value] = key;
  }
  return inverted;
}
```

- [Highest and Lowest](https://www.codewars.com/kata/highest-and-lowest/javascript)

```
function highAndLow(numbers){
  let newNumbers = numbers.split(' ')
 return `${Math.max(...newNumbers)} ${Math.min(...newNumbers)}`
}
```

# Easy Katas Modulo 3

- [Complementary DNA](https://www.codewars.com/kata/complementary-dna/javascript)

```function DNAStrand(dna) {
  complement = '';
   dna.split('').forEach((letter)=>{
    switch (letter) {
      case 'A':
        complement += 'T';
        break;
      case 'T':
        complement += 'A';
        break;
      case 'C':
        complement += 'G';
        break;
      case 'G':
        complement += 'C';
        break;
    }
   })


  return complement;
}
```

- [Descending Order](https://www.codewars.com/kata/descending-order/train/javascript)

```
function descendingOrder(n){
return [...n+''].sort().reverse().join('')*1
}
```
