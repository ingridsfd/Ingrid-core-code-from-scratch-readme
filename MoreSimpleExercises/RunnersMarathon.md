# August 4, 2022
## Runners and registration exercise

A problem where we need the computer to tell us what is our time to race, assigning the values of age and whether we registered early or not:
This is the solution:
```JavaScript
//This variable will allow me to stablish the amount of runners.
let raceNumber = Math.floor(Math.random() * 1000);
//step 2 is set the variable whether is true or not. Did they sign in early or not? set the tone to true or false.
const earlyRunner = false;
//step 3 set all runner's age, it's about more or less from 18.
const age = 18;
//setp 4 here starts the control flow
if (earlyRunner && age > 18) {
  raceNumber += 1000;
}
//step 5 the target is to assign the runners through printing, the hour they will start their race
if (earlyRunner && age > 18){ 
  console.log(`Race starts at 9:30, your race number is: ${raceNumber}.`);
}
//step6 
else if (!earlyRunner && age > 18){
  console.log(`Race starts at 11:00, your race number is: ${raceNumber}.`);
}
//step7
else if (age < 18) {
  console.log(`Race starts at 12:30, your race number is: ${raceNumber}.`);
}
//step 8 modify and verify it runs with several different values
else {
  console.log('Please approach the registration desk, thanks!.');
}
```
