## These are practices of array methods from CodeCademy:
```JavaScript
const groceryList = ['orange juice', 'bananas', 'coffee beans', 'brown rice', 'pasta', 'coconut oil', 'plantains'];
//
groceryList.shift();
//step1
groceryList.unshift('popcorn');
//step2
console.log(groceryList);
//step 3  .slice() is non-mutating function
console.log(groceryList.slice(1,4));
//step 4
console.log(groceryList);
//step 5
const pastaIndex = groceryList.indexOf('pasta');
console.log(pastaIndex);
```
## This prints each value in the array:
```JavaScript
const vacationSpots = ['Bali', 'Paris', 'Tulum'];
// Write your code below
for (let i = 0; i < vacationSpots.length; i++) {
  console.log('I would love to visit' + vacationSpots[i]);
}
```
## Methods available for Arrays according to CodeCademy:
```JavaScript
const cities = ['Orlando', 'Dubai', 'Edinburgh', 'Chennai', 'Accra', 'Denver', 'Eskisehir', 'Medellin', 'Yokohama'];

const nums = [1, 50, 75, 200, 350, 525, 1000];

//  Choose a method that will return undefined
cities.forEach(city => console.log('Have you visited ' + city + '?'));

// Choose a method that will return a new array
const longCities = cities.filter(city => city.length > 7);

// Choose a method that will return a single value
const word = cities.reduce((acc, currVal) => {
  return acc + currVal[0]
}, "C");

console.log(word)

// Choose a method that will return a new array
const smallerNums = nums.map(num => num - 5);

// Choose a method that will return a boolean value
nums.every(num => num < 0);
```
## Definitions review of some methods:

* .forEach() is used to execute the same code on every element in an array but does not change the array and returns undefined.
* .map() executes the same code on every element in an array and returns a new array with the updated elements.
* .filter() checks every element in an array to see if it meets certain criteria and returns a new array with the elements that return truthy for the criteria.
* .findIndex() returns the index of the first element of an array that satisfies a condition in the callback function. It returns -1 if none of the elements in the array satisfies the condition.
* .reduce() iterates through an array and takes the values of the elements and returns a single value.
All iterator methods take a callback function, which can be a pre-defined function, a function expression, or an arrow function.
