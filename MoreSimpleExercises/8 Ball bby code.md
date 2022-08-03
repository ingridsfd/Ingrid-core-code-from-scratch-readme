# This is the code for a 8 Ball simulation
## August 3rd, 2022
Baby exercises that will help me understand better the ones we are doing during CoreCode: 

```JavaScript
//step 1
let userName = 'Ingrid';
//step 2
userName ? console.log(`Hello, ${userName}!`) : console.log('Hello!');
//step 3
let userQuestion = 'will I find love?';
//step 4
console.log(`${userName} has asked - ${userQuestion}`);
//step 5
let randomNumber = Math.floor(Math.random() * 8);
console.log(randomNumber);
//step 6
let eightBall = '';
//step7
switch(randomNumber) {
  case 0:
    eightBall = 'It is certain';
    break;
  case 1:
    eightBall = 'It is decidedly so';
    break;
  case 2:
    eightBall = 'Reply hazy try again';
    break;
  case 3:
    eightBall = 'Cannot predict now';
    break;
  case 4:
    eightBall = 'Do not count on it';
    break;
  case 5:
    eightBall = 'My sources say no';
    break;
  case 6:
    eightBall = 'Outlook not so good';
    break;
  case 7:
    eightBall = 'Signs point to yes'
    break;
}
//step 8
console.log(`The Magic 8 Ball says, ${eightBall}.`)
//step 9 run the program
```
