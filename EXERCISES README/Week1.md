# Week Challenges

## Tuesday 19 July, 2022

1. [x] **Base on this reading and this video, create an explanation about Interpreted And Compiled Programming Languages in your README.
  Interpreted and Compiled Programming Languages.**
  
  **Overall Explanation:** Programs need to be run by general CPU hardwares.
  Depending on the main target or function of a software or application, we might choose between 3 archetypes of programming languages for working in their development or testing:
  1. Compiling the source code: These are the files and codes that do not move easily from one computer device to another to work on it.
    Program examples: C, C++, Objective-C.
  2. Interpreting code: These are the files and codes that do move more freely from device to device to work on them.
    Examples are: PHP, JavasScript.
  3. Just in time or Jit Compilation: Is when the files of the coding achieve the longest expansion between several 'flexible' devices.
  Examples of Hybrid programs: Java, C#, VB.NET, Python. (swift, PHP?)
  
2. [x] **Is Java compiled or interpreted, or both?, check the sources and answer the question in your README.**
    Answer: It's an hybrid so it's possible to be run by a hardware CPU.
    Mainly, it turns the
    - **Machine language:** binary code (compiled languages)
    into
    - **Human language:** Coding and programming (assembly language).
    Bytecode: abstract code, that machine language reads. Is treated like a binary file. 
  Are there any software examples of these archetypes?
    
3. [x] **Pseudocode Currency Converter exercise.**
**Steps in my own words:**
   Definition of the algorithm: To convert dollars (USD) to bitcoin (BTC).
   1. Read the dollar rate.
   2. Search for the last updated bitcoin rate.
   3. Read bitcoin rate.
   4. Multiply dollar rate value * the last updated bitcoin rate value.
   5. Result - Output.
**Steps in algorithm language would be:**
```
  Starting point: START
  READ dollar rate
  Input: GET last updated bitcoin rate (https://www.coindesk.com/price/bitcoin/)
  READ
  PRINT dollar Rate * Bitcoin rate
  Assignation: <-- lo que teclea el usuario es llevado al programa 
  End point: END
 ```

4. [x] **Learn about High and Low level languages.**
```
    **Notes:** 
    Assembly language: hardware redabale language.
    Machine code: binary.
    Programs like COBOL, Fortran are way too abstract.
    Rely better on functions. Fox example, C > Assembly is low level language. Python > C is low level.
```

## Wednesday 20 July, 2022

1. [x] **Your date of birth in the matrix? exercise.**


| Birth Date      | Binary Code |
| -----------     | ----------- |
| 14.10.1997      | 1110.1010.  |
| Year in binary  |11111001101  |
 

2. [x] **MIPS exercise.**
Instructions
1. Create a program that adds any two given numbers provided by the user. Code pasted from Mars 4.5:
```
  .data
	      number1: .asciiz "\nIngrese el primer numero: "
	      number2: .asciiz "\nIngrese el segundo numero: "
  .text
	      main:
              li $v0, 4
              la $a0, number1
              syscall

              li $v0, 5
              syscall

              move $t0, $v0

              li $v0, 4
              la $a0, number2
              syscall

              li $v0, 5
              syscall

              move $t1, $v0

              li $v0, 1
              move $a0, $t0
              syscall
```
```      
 .data
	      result_message: .asciiz "\nEl resultado es: "
  .text
	      
              li $t0, 30
              li $t1, 50

              add $t2, $t0, $t1

              li $v0, 4
              la $a0 result_message
              syscall

              li $v0, 1
              move $a0, $t2
              syscall
```
CODE FIXED AFTER CONSULTING IN CLASS:
``` 
.data
	      number1: .asciiz "\nIngrese el primer numero: "
	      number2: .asciiz "\nIngrese el segundo numero: "
	      result_message: .asciiz "\nEl resultado es: "
	      message: .asciiz "\nIngrid Fonoy\n"
  .text
  	main:
              li $v0, 4
              la $a0, number1
              syscall

              li $v0, 5
              syscall

              move $t0, $v0

              li $v0, 4
              la $a0, number2 
              syscall

              li $v0, 5
              syscall

              move $t1, $v0

              add $t2, $t0, $t1

              li $v0, 4
              la $a0 result_message
              syscall

              li $v0, 1
              move $a0, $t2
              syscall

              li $v0, 4
              la $a0, message
              syscall
``` 

2. Create a program that displays your name. Code pasted from Mars 4.5:
```
  .data
        message: .asciiz "\nIngrid Fonoy\n"
  .text
        main:
              li $v0, 4
              la $a0, message
              syscall
```
## Thursday 21 July, 2022

1. [x] Print special numbers exercise.
**Exercise Description** 
In this exercise you must use an iterative flow control to be able to print all the even numbers in the range of numbers from 0 to 100. Remember that you should not print each number, you should use a flow control structure to perform the exercise.

Even numbers are: 2, 12, 22, 32, 42, 52, 62, 72, 82, 92, 4, 24...100
My code answer: 
```javascript
let str = '';

for (let i = 0; i <= 100; i++) {
  if (i % 2 == 0)

console.log(i);
}
```
3. [x] Bad Code exercise.
**Exercise Description**
The code shown below is not working in the right way, as a task you must find the error made by the developer who programmed this code and correct it, for this exercise you must explain what the error is and place the correct code.
```Javascript
var cond = false;

if ((cond = true)) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
}
```
Fixed code would be:
```Javascript
var cond = false;

if (cond == true) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
}
```
**Answer Description:**
Considering the fact that we want to print the variable 'false' in the first place, it ends up printing the opposite, and it's not considering the right instruction to print it.

5. [x] Bad Code 2 exercise.
**Exercise Description**
You must create the code that follows the following logic, if the given number is 100, take this number as special and show the following message: "This is a special number!", but if the number is less than 1000, multiple of 10 and different from 100, you must show the following message: "This number is almost special". if none of the given conditions are met show the following message: "Just a regular number". Another developer was trying to program the logic, but apparently couldn't, you need to fix the code to work properly
```Javascript
var n = 100;

if (n == 100) {
  console.log('This is a special number!');
}
if (n < 1000) {
  console.log('');
} else {
  console.log('Just a regular number');
}
if (n % 10 == 0) {
  console.log('This number is multiple of 10');
}
```
FIXED CODE WOULD BE:
```Javascript
var n=100;
if(n==100) {
  console.log('This is a special number!');
} else
if(n<100 && n%10 == 0 && n!=1000){
  console.log('This number is almost special');
  }
  else{
  console.log('Just a regular number');
  }
```
7. [pending] Follow Git Course.
Tracking progress:
1. [x] Part 1
2. [x] Part 2
3. [x] Part 3
4. [x] Part 4
5. [ ] Part 5
6. [x] Part 6
