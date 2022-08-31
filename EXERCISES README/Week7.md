# Week challenges (Monday) 💻
1. [x] Watch Object Oriented Programming - The Four Pillars of OOP

Surrounds the topics of
* Abstraction: Show the user only the necessary details
* Inheritance: code reusability
* Polymorphism: Determina which functions to run while the programm is running
* Encapsulation: setting to private certain properties to still encapsulate within the object

3. [x] Readme - OOP exercise

Definitons of the main concepts:

* Class: Set of instructions.
* Object: File that contains the properties or characteristics.
* Instance: When data is assigned and called along the object.
* Interface: Is the variables and data that holds within the blocks. Lives in the memory. You don't have to have a class created.
* Access Modifiers: It's where we can get and set more that to the values stablished already.
* Constructors: is where we define the parameters for values for the instance or static properties.
* Methods: are behaviours or actions.

Example [insert example here]


# Week challenges (Tuesday) 💻
3. [x] Input/Output playground, using Typescript

# Week challenges (Wednesday) 💻
4. [ ] Build Tower exercise, using Typescript
5. [ ] Meeting exercise, using Typescript

# Week challenges (Thursday) 💻
6. [x] Interfaces guided exercise, using Typescript
```JavaScript
//About using TypeScript interfaces
interface IceCream {
  flavor: string;
  scoops: number;
  instructions?: string;
}

let myIceCream: Sundae = {
  flavor: 'vanilla',
  scoops: 2,
  sauce: 'caramel',
  nuts: true
}
console.log(myIceCream.flavor);

function tooManyScoops(dessert: Sundae) {
  if (dessert.scoops >= 4) {
    return dessert.scoops + ' is too many scoops!';
  } else {
    return 'Your order will be ready soon!';
  }
}

console.log(tooManyScoops({flavor: 'vanilla', scoops: 5, sauce: 'caramel'}));
//extend the interface
interface Sundae extends IceCream {
  sauce: 'chocolate' | 'caramel' | 'strawberry';
  nuts?: boolean;
  whippedCream?: boolean;
  instructions?: string;
}
```
Declaring and implementing interfaces
```JavaScript
/* Module 3: Implement interfaces in TypeScript
   Lab Start  */

/*  EXERCISE 1
    TODO: Declare the Loan interface. */
interface Loan {
    principal: number,
    interestRate: number
}

/*  TODO: Declare the ConventionalLoan interface. */
interface ConventionalLoan extends Loan {
    months: number
}


/*  TODO: Update the calculateInterestOnlyLoanPayment function. */
function calculateInterestOnlyLoanPayment(loanTerms: Loan): string {
    let interest = loanTerms.interestRate / 1200;
    let payment;
    payment = loanTerms.principal * interest;
    return 'The interest only loan payment is ' + payment.toFixed(2);
}

let interestOnlyPayment = calculateInterestOnlyLoanPayment({ principal: 30000, interestRate: 5 });
console.log(interestOnlyPayment);

/*  TODO: Update the calculateConventionalLoanPayment function. */

function calculateConventionalLoanPayment(loanTerms: ConventionalLoan): string {
    // Calculates the monthly payment of a conventional loan
    let interest: number = loanTerms.interestRate / 1200; // Calculates the Monthly Interest Rate of the loan
    let payment: number;
    payment = loanTerms.principal * interest / (1 - (Math.pow(1 / (1 + interest), loanTerms.months)));
    return 'The conventional loan payment is ' + payment.toFixed(2);
}

let conventionalPayment = calculateConventionalLoanPayment({ principal: 30000, interestRate: 5, months: 180 });
console.log(conventionalPayment)

//let interestOnlyPayment = calculateInterestOnlyLoanPayment(30000, 5);
//let conventionalPayment = calculateConventionalLoanPayment(30000, 5, 180);

//console.log(interestOnlyPayment);     //* Returns "The interest only loan payment is 125.00" 
//console.log(conventionalPayment);     //* Returns "The conventional loan payment is 237.24" 
```

8. [x] ✨Complete your 4th Core Challenge. This is one of the requirements for the certification, where you'll boost your dev professional-brand.

# Extra (It is not mandatory for the Readme) ⭐
8. [ ] Menu exercise, using Typescript
