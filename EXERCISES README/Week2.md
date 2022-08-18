# Week Challenges

## Monday 25 July, 2022
1. [x] Create an account in Codewars, follow the instructions.
2. [x] Read about if...else.

Notes:
- Most comfortable to work with }{.
- If...else use a space between them.
- When using true - false do not confuse with Boolean.

4. [x] Read about: for

Notes:
- To create loops in a statement.
- Usually in a block statement.
6. [x] Read about: while.

Notes:
- Creates a loop as long as it evaluates it as 'true'.
8. [x] Read about: functions.

Notes:
- Function declaration is where you declare parameters, names, and operations.
- It's the insertion of an instruction.
## Tuesday 26 July, 2022
1. [x] Start this HTML course.
3. [x] Multiply exercise.
```JavaScript
function multiply(a, b){
  let c = a * b
  return c; 
}
```
5. [x] ASCII Total exercise.
```JavaScript
function uniTotal(str) {
  let total = 0;
  for (let i = 0, length = str.length; i < length; i++) {
    total += str[i].charCodeAt();
  }
  return total;
}
```

## Wednesday 27 July, 2022
1. [x] Follow up with the HTML course you started on Tuesday.
2. [x] Char From ASCII Value exercise.

```JavaScript
function getChar(c){
  return String.fromCharCode(c);
}
```
4. [x] Binary Adition Exercise.
```JavaScript
function addBinary(a,b) {
  return (a + b).toString(2); 
}
```
6. [x] Student's Final Grade exercise.
```JavaScript
function finalGrade (exam, projects) {
  let result = 0;
  if (exam > 90 || projects > 10) {
    result = 100;
  } else 
    if (exam > 75 && projects >= 5) {
      result = 90;
    } else
      if (exam > 50 && projects >= 2) {
        result = 75;
      }
        return result // final grade
        }
```
## Thursday 28 July, 2022
1. [x] Follow up with the HTML course you started on Tuesday.
2. [x] Remove All Exclamation Marks From The End Of Sentence exercise
```JavaScript
function remove (string) {  
  let result = '';
  let exclamationMark = string.length - 1;
  for (let i = exclamationMark; i > 0; i--){
    if (string[i] !== '!') {
      result = string.substring(0, i + 1);
      break;
    }
  }
  return result;
}
```
4. [x] Vowel Remover exercise
```JavaScript
function shortcut(string) {
  let result = '';
  for (let i = 0; i < string.length; i++) {
    if (string[i] == 'a' || string[i] == 'e' || string[i] == 'i' || string[i] == 'o' || string[i] == 'u') {
      continue;
    }
    result = result + string[i];
  }
  return result;
}
```
6. [x] Rock Paper Scissors! exercise. Here we learn to call a functions througn the 'fat arrow' =>
```JavaScript
const rps = (p1, p2) => {
  if (p1 === p2) return 'Draw!';
  if (p1 === 'rock' && p2 === 'scissors') return 'Player 1 won!';
  if (p1 === 'scissors' && p2 === 'paper') return 'Player 1 won!';
  if (p1 === 'paper' && p2 === 'rock') return 'Player 1 won!';
  return 'Player 2 won!';
};
```
8. [x] Persistent Bugger exercise
```JavaScript
function persistence(num) {
  let numString = num.toString();
  let cantDigits = numString.length;

  if (cantDigits == 1) {
    return 0;
  }
  
  let i = 0;
  let mult = 0;
  for(; cantDigits >= 2; i++) {

    mult = 1;
    for(let j = 0; j < numString.length; j++) {
      mult = Number(mult) * Number(numString[j]);
    }
    numString = mult.toString();
    cantDigits = numString.length;
  }
  
  return i;
}
```
## Extra exercises (not mandatory for the README)
1. [ ] Holiday VIII - Duty Free exercise
2. [x] Twice As Old exercise
```JavaScript
function twiceAsOld(dadYearsOld, sonYearsOld) {
  //How many years ago //the father was 2twice as old as his son
  let twiceAge = sonYearsOld * 2;
  //how many years he will be twice as old
  let difference = dadYearsOld - twiceAge;
  return Math.abs(difference);
}
```
4. [x] Valid Spacing exercise
```JavaScript
function validSpacing(s) {
    if(s.charAt(0) === ' ' || s.charAt(s.length - 1) === ' ') { 
     return false;
  }
  
  for(let i = 0; i < s.length; i++) {
    if(s.charAt(i) === ' '){ 
      if(i != 0 && s.charAt(i-1) === ' ') {
        return false;
      }
      if(i != (s.length - 1) && s.charAt(i+1) === ' ') {
        return false;
      }
    }
    // ....
  }
  
  return true; //...
}
```
6. [ ] Fake Binary exercise
