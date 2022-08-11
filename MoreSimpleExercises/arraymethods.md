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
