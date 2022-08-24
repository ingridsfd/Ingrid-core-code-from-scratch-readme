# Week challenges (Monday) 💻
1. [x] Declare variable types in TypeScript guided exercise, using Typescript
```Typescript
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
4. [ ] TypeScript Unions exercise
# Week challenges (Tuesday) 💻
4. [ ] Square(n) Sum exercise, using Typescript
5. [ ] Growth Of A Population exercise, using Typescript
6. [ ] Mumbling exercise, using Typescript
7. [ ] A Wolf In Sheep's Clothing exercise, using Typescript
# Week challenges (Wednesday) 💻
8. [ ] A Rule Of Divisibility By 13 exercise, using Typescript
9. [ ] Playing With Digits exercise, using Typescript
10. [ ] Valid Braces exercise, using Typescript
11. [ ] Tic-Tac-Toe exercise, using Javascript
12. [ ] Tic-Tac-Toe-Like Table Generator exercise, using Javascript
# Week challenges (Thursday) 💻
13. [ ] Declare and instantiate classes in TypeScript guided exercise, using Typescript
14. [ ] Tile exercise, using Typescript
15. [ ] Time exercise, using Typescript
16. [ ] Rational exercise, using Typescript
