Today in class we covered a topic of functional programing and how declarative
functions are much more cleaner, efficient and process faster. Imperative functions
take up more lines of code which then takes longer to process, and longer to write it out.

WHAT: you want (declarative)
HOW: The steps to get it done (imperative)

Here are examples of the Imperative vs Declarative functions that have the same functionality:

Imperative
```
var nums = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10];

function smallEvens(arr) {
  var output = [];
  arr.forEach(function(ele) {
    if (ele < 5 && ele % 2 === 0) {
      output.push(ele);
    }
  })
  return output;
}
```
Declarative
```
let smallEvensArrow = nums.filter( num => num < 5 && num % 2 === 0 )
```
Functional features built in to JavaScript and most commonly used array methods that do not "mutate" (dont change) the data:
```
forEach (applies function once per element)
.some and .every (returns a boolean)
.concat (returns new array - think push(), but without side-effects!)
.filter (returns new array of values based on boolean results)
.map (returns new array of values based on the function applied)
.reduce (return new value based on the accumulator set)
```
Its always good practice to avoid methods that "mutate" (change) data such as:
```
.sort()
.reverse()
.splice()
```
