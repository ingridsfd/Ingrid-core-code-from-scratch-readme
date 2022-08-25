# Monday 22 august, 2022
1. [x] Declare variable types in TypeScript guided exercise, using Typescript
```TypeScript
/*  EXERCISE 1
    TODO: Modify the code to add types to the variable declarations. 
    The resulting JavaScript should look the same as the original example when you're done. */

let firstName: string;
let lastName: string;
let fullName: string;
let age: number;
let ukCitizen: boolean;

firstName = 'Rebecca';
lastName = 'Smith';
age = 42;
ukCitizen = false;
fullName = firstname + " " + lastname;

if (ukCitizen) {
    console.log("My name is " + fullName + ", I'm " + age + ", and I'm a citizen of the United Kingdom.");  
} else {
    console.log("My name is " + fullName + ", I'm " + age + ", and I'm not a citizen of the United Kingdom.");
}

/* EXERCISE 2
   TODO: You can use types to ensure operation outcomes. Run the code as is and then modify 
   it to have strongly typed variables. Then, address any errors you find so that the result 
   returned to a is 12. */

let x: number;
let y;
let a;

x = 5;
y = 7;
a = x + y;

console.log(a);

/* EXERCISE 3
   TODO: In the following code, implement an enum type called Season that represents 
   the constants "Fall", "Winter", "Spring", and "Summer". Then, update the function so 
   you can pass in the season by referencing an item in the enum, for example 
   Season.Fall, instead of the literal string "Fall". */

enum Season {
    Winter,
    Spring,
    Summer,
    Fall
};

function whichMonths(season: Season) {

    let monthsInSeason: string;

    switch (season) {
        case Season.Fall:
            monthsInSeason = "September to November";
            break;
        case Season.Winter:
            monthsInSeason = "December to February";
            break;
        case Season.Spring:
            monthsInSeason = "March to May";
            break;
        case Season.Summer:
            monthsInSeason = "June to August";
    }

    return monthsInSeason;
}

console.log(whichMonths(Season.Fall));

/* EXERCISE 4
   TODO: Declare the array as the type to match the type of the items in the array. */

   let randomNumbers: number[] = [];
   let nextNumber: number;
   
   for (let i = 0; i < 10; i++) {
       nextNumber = Math.floor(Math.random() * (100 - 1)) + 1;
       randomNumbers.push(nextNumber);
   }
   
   console.log(randomNumbers);
```
3. [x] TypeScript Object Type exercise
```TypeScript
 /* EXERCISE 1
 Intro context for the exercise:

    We are starting a small community of users. For performance
    reasons we have decided to store all users right in the code.
    This way we can provide our developers with more
    user-interaction opportunities. With user-related data, at least.
    All the GDPR-related issues will be solved some other day.
    This would be the base for our future experiments during
    these exercises.

Exercise:

    Given the data, define the interface "User" and use it accordingly.

*/

export interface User {
    name: string;
    age: number;
    occupation: string;
}

export const users: User[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    }
];

export function logPerson(user: User) {
    console.log(` - ${user.name}, ${user.age}`);
}

console.log('Users:');
users.forEach(logPerson);
```
5. [x] TypeScript Unions exercise
### Exercise to define the type of Person: User | Admin
```TypeScript
/* EXERCISE 2

Intro:

    All 2 users liked the idea of the community. We should go
    forward and introduce some order. We are in Germany after all.
    Let's add a couple of admins.

    Initially we only had users in the in-memory database. After
    introducing Admins, we need to fix the types so that
    everything works well together.

Exercise:

    Type "Person" is missing, please define it and use
    it in persons array and logPerson function in order to fix
    all the TS errors.

*/

interface User {
    name: string;
    age: number;
    occupation: string;
}

interface Admin {
    name: string;
    age: number;
    role: string;
}

export type Person = User | Admin;

export const persons: Person[] = [
    {
        name: 'Max Mustermann',
        age: 25,
        occupation: 'Chimney sweep'
    },
    {
        name: 'Jane Doe',
        age: 32,
        role: 'Administrator'
    },
    {
        name: 'Kate Müller',
        age: 23,
        occupation: 'Astronaut'
    },
    {
        name: 'Bruce Willis',
        age: 64,
        role: 'World saver'
    }
];

export function logPerson(user: Person) {
    console.log(` - ${user.name}, ${user.age}`);
}

persons.forEach(logPerson);
```
# Tuesday 23 august, 2022
1. [x] Square(n) Sum exercise, using Typescript
```JavaScript
export function squareSum(numbers: number[]): number {
  //1. Turn numbers to squared ^2
  //const squaredNums = Math.pow(1, 2);
  // 2. Sum the numbers once squared with .reduce()
  return numbers.reduce((prev: number, curr: number) => prev + Math.pow(curr, 2), 0);
}
```
3. [x] A Wolf In Sheep's Clothing exercise, using Typescript
```JavaScript
export function warnTheSheep(queue: string[]): string {
  //1. establish the wolf location
  let wolfP = queue.indexOf('wolf');
  //2. put the conditionals to return 'go away' or 'alert the sheep'
  if(wolfP == queue.length - 1) {
    return 'Pls go away and stop eating my sheep';
} else {
  return `Oi! Sheep number ${Math.abs(wolfP + 1 - queue.length)}! You are about to be eaten by a wolf!`
}
};
```
# Wednesday 24 august, 2022
1. [ ] A Rule Of Divisibility By 13 exercise, using Typescript
2. [x] Playing With Digits exercise, using Typescript
```JavaScript
export class G964 { //excuse the spanglish

    public static digPow = (n: number, p: number) => {
      let sum =
      //1. Convertir primero a string, porque solo está en num hasta ahorita
      n.toString()
      //2. Hay que convertir de string a array porque .map solo utiliza arrays
      .split('')
      //3. find a positive integer k * n = a^(n)+b^(n+1)+c^(n+2);
      .map(Number)
      //4. haz la suma de cuando ya tengas cada numero expresado a su correspondiente potencia
      .reduce((prev: number, curr: number) => prev + Math.pow(curr, p++), 0);
      //5. if the positive integer is correct, return k. always a positive number is using Math.abs(n);
      if (sum % n === 0) return sum / n; //se podría haber utilizado Math.abs() para designar el num positivo?
      //6. if not, return -1
      else return -1;
    }
}
```

# Thursday 25 august, 2022
1. [x] Declare and instantiate classes in TypeScript guided exercise, using Typescript
### Create a Class
```JavaScript
class Car {
    // Properties
    _make: string;
    _color: string;
    _doors: number;

    //Constructor
    constructor(make: string, color: string, doors = 4) {
        this._make = make;
        this._color = color;
        this._doors = doors;
    }
    //Accessors
    get make() {
        return this._make;
    }
    set make(make) {
        this._make = make;
    }
    get color() {
        return 'The color of the car is ' + this._color;
    }
    set color(color) {
        this._color = color;
    }
    get doors() {
        return this._doors;
    }
    set doors(doors) {
        if((doors % 2) === 0) {
            this._doors = doors;
        } else {
            throw new Error('Doors must be an even number');
        }
    }

    //Methods
    accelerate(speed: number): string {
        return `${this.worker()} is accelerating to ${speed} MPH.`
    }
    brake(): string {
        return `${this.worker()} is braking with the standard braking system.`
    }
    turn(direction: 'left' | 'right'): string {
        return `${this.worker()} is turning ${direction}`;
    }
    worker(): string {
        return this._make;
    }
}

let myCar1 = new Car('Cool Car Company', 'blue', 2);
console.log(myCar1.color);

let myCar2 = new Car('Galaxy Motors', 'red', 3);

let myCar3 = new Car('Galaxy Motors', 'gray');
console.log(myCar3.doors);

console.log(myCar1.accelerate(35));
console.log(myCar1.brake());
console.log(myCar1.turn('right'));
```
3. [ ] Tile exercise, using Typescript
4. [ ] Time exercise, using Typescript
5. [ ] Rational exercise, using Typescript
