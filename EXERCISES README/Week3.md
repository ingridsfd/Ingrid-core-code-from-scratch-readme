# Week Challenges

## Monday august 1, 2022
1. [x] Who Likes It? exercise
```JavaScript
let names= ["John", "Mark"]
function likes(names) {
    switch(names.length) {
    case 0:
        return 'no one likes this';
        break;
    case 1:
        return names[0] +  ' likes this';
        break;
    case 2:
        return names[0] + ' and '+ names[1] + ' like this';
        break;
    case 3:
        return names[0]+', '+ names[1] + ' and ' + names[2] + ' like this';
        break;
    default:
        return names[0]+ ', '+ names[1] + ' and ' + (names.length-2 ) + ' others like this';
        break;
    }
}
console.log(likes(names) );
```
3. [x] Bit Counting exercise
```JavaScript
var countBits = function(n) {
  var binaryNum = n.toString(2);
  let bit = 0;
  for (i = 0; i < binaryNum.length; i++) {
    if (binaryNum[i] === '1') bit++;
  }
  return bit;
};
```
6. [ ] Your Order, Please exercise

## Tuesday august 2, 2022
4. [x] Simple Pig Latin exercise.

Forgot to put REGEX of space in the last string which is --| $-- to considerate the last space of the string. [fixed]
```JavaScript
function pigIt(str){
  return str.replace (/(\w)(\w*)(\s|$)/g, '$2$1ay$3');
}
```

6. [x] Counting Duplicates exercise
```JavaScript
function duplicateCount(text){
  // Ii (case sensitive, son diferentes)
  // Ii (case insensitive, son igual)
  let duplicates = 0;
  text = text.toLowerCase(); // todo minuscula
  for(let i = 0; i < text.length; i++) {
    if(text.indexOf(text[i]) !== text.lastIndexOf(text[i])) {
      duplicates++;
      text = text.replace(new RegExp(`${text[i]}`, 'g'), '');
      i = i-1;
    }
  }
  return duplicates;
}
```
7. [ ] Decode The Morse Code exercise

## Wednesday august 3, 2022
7. [ ] Valid Parentheses exercise
8. [ ] Convert String To Camel Case exercise
9. [ ] Unique In Order exercise

## Thursday august 4, 2022
8. [ ] Fold An Array exercise
9. [ ] Encrypt This! exercise
```JavaScript
var encryptThis = function (text) {
    //code here
}
// [hello, world]
let str = 'world';
let charBackup = str[1];
// 1
/*
  W0[0].charCodeAt(0) 
*/
str = str.replace(str[0], str.charCodeAt(0));
// 2
/*
 W0[1] = W0[W0.length-1]
 W0[W0.length-1] = W0[1]
*/
//str = str.replace(charBackup, str[str.length-1]);
//str = str.replace(/\w$/, charBackup);

str = str.slice(0, str.length-1) + charBackup;
//str = `${str.slice(0, str.length-1)}${charBackup}`;
//str = str.slice(0, str.length-1).concat(charBackup);

console.log(str); 
```
11. [x] ✨Complete your 1st Core Challenge. This is one of the requirements for the certification, where you'll boost your dev professional-brand.
