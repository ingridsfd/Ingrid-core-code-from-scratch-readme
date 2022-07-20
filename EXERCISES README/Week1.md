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
  Starting point: START
  READ dollar rate
  Input: GET last updated bitcoin rate (https://www.coindesk.com/price/bitcoin/)
  READ
  PRINT dollar Rate * Bitcoin rate
  Assignation: <-- (??) se usa igual que el símbolo de "="?? DUDA
  End point: END
 
4. [x] **Learn about High and Low level languages.**
    **Notes:** 
    Assembly language: hardware redabale language.
    Machine code: binary.
    Programs like COBOL, Fortran are way too abstract.
    Rely better on functions. Fox example, C > Assembly is low level language. Python > C is low level.

## Wednesday 20 July, 2022

1. [x] **Your date of birth in the matrix? exercise.**
My birthday is October 14, 1997 = 14/10/1997.
**Answer in binary numbers: 1110 | 1010 | 11111001101**
 
2. [x] **MIPS exercise.**
Instructions
1. Create a program that adds any two given numbers provided by the user. Code pasted from Mars 4.5:
 .data
	      number1: .asciiz "\nIngrese el primer numero: "
	      number2: .asciiz "\nIngrese el segundo numero: " 
	      number3: .asciiz "\nLa suma es: " 
  .text
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
              
              add $t1, $t2, $t3
              
              li $v0,4
              la $a0,number3
              syscall
              
              li $v0,1
              la $a0,($t2)
              syscall


2. Create a program that displays your name. Code pasted from Mars 4.5:

  .data
        message: .asciiz "\nIngrid Fonoy\n"
  .text
        main:
              li $v0, 4
              la $a0, message
              syscall

## Thursday 21 July, 2022

1. [ ] Print special numbers exercise.
2. [ ] Bad Code exercise.
3. [ ] Bad Code 2 exercise.
4. [ ] Follow Git Course.
