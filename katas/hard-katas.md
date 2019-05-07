# Hard Katas Modulo 1

- [Number of anagrams in an array of words](https://www.codewars.com/kata/587e18b97a25e865530000d8)

```
function anagramCounter (wordsArray) {
  var counter = 0;
  var wordSorted = wordsArray.map((word)=>{return[...word].sort().join("");}).forEach((word, i, wordSorted)=>{
    for (var j = i; j < wordSorted.length; j++) {
      if(wordSorted[i] === wordSorted[j+1]) counter++
    };
  })
  return counter;
}

```

- [TGI Friday!!](https://www.codewars.com/kata/5a0d6d8c6975982b5b000383)

```
function lastDayIsFriday(initialYear, endYear) {
  var finalYear = endYear || initialYear
  var fridayCounter = 0;

  for (var year = initialYear; year <= finalYear; year++){
      for (var month = 1; month <= 12; month++){
          var date = new Date (year, month, 0);
          if(date.getDay() === 5) {
          fridayCounter++;
      };
    }
  }
return fridayCounter
}
```

//TODO: @manu

- [Clocky Mc Clock-Face](https://www.codewars.com/kata/clocky-mc-clock-face/javascript)

- [Sort a 2D array](https://www.codewars.com/kata/587f46c9406f2dc381000009)

```
function namesSorter (departmentsArray) {
  return [].concat.apply([],departmentsArray).sort((a,b) => a.length - b.length || a.localeCompare(b))
}
```

//TODO: @Manu @Alex

- [Persistent Bugger.](https://www.codewars.com/kata/persistent-bugger)
  //TODO: @manu @alex
- [Find the missing letter](https://www.codewars.com/kata/find-the-missing-letter/javascript)
  //TODO: @manu @alex
- [Street Fighter 2 - Character Selection](https://www.codewars.com/kata/street-fighter-2-character-selection/javascript)
  //TODO: @manu @alex
- [Playing with digits](https://www.codewars.com/kata/playing-with-digits/javascript)

- [Sum of Pairs](https://www.codewars.com/kata/sum-of-pairs/javascript)

```
var sum_pairs=function(ints, s){
  var seen = {}
  for (var i = 0; i < ints.length; ++i) {
    if (seen[s - ints[i]]) return [s - ints[i], ints[i]];
    seen[ints[i]] = true
  }
}
```

//TODO: @manu @alex

- [All that is open must be closed...](https://www.codewars.com/kata/all-that-is-open-must-be-closed-dot-dot-dot/javascript)
  //TODO: @manu @alex
- [Directions Reduction](https://www.codewars.com/kata/directions-reduction/)
  //TODO: @manu @alex
- [Scramblies](https://www.codewars.com/kata/scramblies/)
  //TODO: @manu @alex
- [Pete, the baker](https://www.codewars.com/kata/pete-the-baker/)
