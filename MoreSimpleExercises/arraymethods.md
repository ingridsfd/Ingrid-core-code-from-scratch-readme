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
