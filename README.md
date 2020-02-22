# Solved-Tasks

[Multiply](https://www.codewars.com/kata/50654ddff44f800200000004/train/javascript)
```javascript
function multiply(a, b){
 return a * b
}
```
[Tail Swap](https://www.codewars.com/kata/5868812b15f0057e05000001/train/javascript/5e2a194602c0950017a11f3f)
```javascript
function tailSwap(arr) {
let arr0 = arr[0].split(':');
let arr1 = arr[1].split(':');
return [arr0[0] + ':' + arr1[1], arr1[0] + ':' + arr0[1]]
}
```

[Count of positives / sum of negatives](https://www.codewars.com/kata/576bb71bbbcf0951d5000044/solutions/javascript)
```javascript
function countPositivesSumNegatives(arr) {
  if (!arr || arr.length === 0 ) return [];
  let countP = 0;
  let sumN = 0;
   for (let i=0; i<arr.length; i++){
    if (arr[i]>0) countP = countP+1;
     else sumN = sumN+arr[i];
   } 
  return [countP, sumN];
}
```
[Calculate average](https://www.codewars.com/kata/57a2013acf1fa5bfc4000921/solutions/javascript/me/best_practice)
```javascript
function find_average(array) {
  // your code here
  return 0;
}

//or
function find_average(arr){
let sum = 0;
for (let i=0; i<arr.length; i++){
sum = sum + arr[i];
}
return sum/arr.length;
}
```
[Divide and counquer](https://www.codewars.com/kata/57eaec5608fed543d6000021/solutions/javascript/me/best_practice)
```javascript
function divCon(x){
  sumN = 0;
  sumS = 0;
   for (let i=0; i<x.length; i++){
    if (typeof x[i] === 'number') sumN = sumN+x[i];
     else sumS = sumS + +x[i];
   } 
   return sumN-sumS;
}
```
[Odd or Even?](https://www.codewars.com/kata/5949481f86420f59480000e7/solutions/javascript/me/best_practice)
```javascript
function oddOrEven(arr){
  let sum = 0;
   for (let i=0; i<arr.length; i++){
    sum = sum+arr[i];
  }
  if (sum%2 === 0) return "even";
  else return "odd";
}
```
[Sum of Odd Cubed Numbers](https://www.codewars.com/kata/580dda86c40fa6c45f00028a/solutions/javascript/me/best_practice)
```javascript
function cubeOdd(arr) {
  let sum = 0;
  for (let i=0; i<arr.length; i++){
   if (typeof (arr[i]) != 'number') return undefined;
   if (arr[i] % 2 != 0) sum = sum + arr[i]**3 
  }
  return sum;
}
```
[How good are you really?](https://www.codewars.com/kata/5601409514fc93442500010b/solutions/javascript)
```javascript
function betterThanAverage(classPoints, yourPoints) {
  let sum = 0;
  for (let i=0; i<classPoints.length; i++){
  sum = sum + classPoints[i]
  }
  return sum/classPoints.length < yourPoints
}
```
[Tail Swap](https://www.codewars.com/kata/5868812b15f0057e05000001/solutions/javascript/me/best_practice)
```javascript
function tailSwap(arr) {
let arr0 = arr[0].split(':');
let arr1 = arr[1].split(':');
return [arr0[0] + ':' + arr1[1], arr1[0] + ':' + arr0[1]]
}
```
[Training JS #1: create your first JS function and print "Helloworld!"](https://www.codewars.com/kata/571ec274b1c8d4a61c0000c8/solutions/javascript)
```javascript
function helloWorld(){
var str = 'Hello World!';
console.log(str);
return str;
}
```
[Function 1 - hello world](https://www.codewars.com/kata/523b4ff7adca849afe000035/solutions/javascript/me/best_practice)
```javascript
function greet(){
var greet = 'Hello World!';
return 'hello world!'
}
```
[Square(n) Sum](https://www.codewars.com/kata/515e271a311df0350d00000f/solutions/javascript/me/best_practice)
```javascript
function squareSum(numbers){
  return numbers.reduce((sum, el) => sum + el * el, 0);
}
// OR
function squareSum(numbers){
  return numbers.reduce(function(sum, n){
    return (n*n) + sum;
  }, 0)
} 
```
[Even or Odd](https://www.codewars.com/kata/53da3dbb4a5168369a0000fe/solutions/javascript/me/best_practice)
```javascript
function even_or_odd(number) {
  if (number % 2 === 0)
    return "Even"
  else
    return "Odd"
}
```
[Find the position!](https://www.codewars.com/kata/5808e2006b65bff35500008f/solutions/javascript/me/best_practice)
```javascript
function position(letter){
  let alphabet = ' abcdefghijklmnopqrstuvwxyz';
  return `Position of alphabet: ${alphabet.indexOf(letter)}`;
}
```
[Add property to every object in array](https://www.codewars.com/kata/54e8c3e89e2ae6f4900005a1/solutions/javascript/me/best_practice)
```javascript
questions.map(el => el.usersAnswer = null);

// OR
for (i=0; i<questions.length; i++) {
questions[i].usersAnswer = null;
};
```
[Coding Meetup #5 - Higher-Order Functions Series - Prepare the count of languages](https://www.codewars.com/kata/5828713ed04efde70e000346/solutions/javascript/me/best_practice)
```javascript
function countLanguages(list) {
let answer = {};
  for(let i = 0; i < list.length; i++){
    if(answer[list[i].language]){
        answer[list[i].language]++;
    } else { 
    answer[list[i].language] = 1;
    }
  } 
return answer
}
```
[Numbers to Objects](https://www.codewars.com/kata/57ced2c1c6fdc22123000316/solutions/javascript/me/best_practice)
```javascript
function numObj(s){
 let res = [];
 for(let i = 0; i < s.length; i++){
 let obj = {};
 obj[s[i]] = String.fromCharCode(s[i]);
 res.push(obj);
 }
 return res
}
```
[What's the real floor?](https://www.codewars.com/kata/574b3b1599d8f897470018f6/solutions/javascript/me/best_practice)
```javascript
function getRealFloor(n) {
  // n <= 0, return 0
  if (n <= 0){
    return n
  // 1 < n < 12, return n-1
  } else if (n <= 12) {
    return n - 1
  // 13 <= n, return n-2
  } else {
    return n - 2
  } 
  
}
```
[Calculate BMI](https://www.codewars.com/kata/57a429e253ba3381850000fb/solutions/javascript/me/best_practice)
```javascript
function bmi(weight, height) {
  let index = weight / height**2;
  if (index <= 18.5)  return "Underweight";
  else 
  if (index <= 25.0) return "Normal"; 
  else 
  if (index  <= 30.0) return "Overweight";
  else return "Obese";
}
// OR
function bmi(w, h) {
  let b = w/Math.pow(h, 2)
  return  b > 30 ? "Obese" :
          b > 25 ? "Overweight" :
          b > 18.5 ? "Normal" : "Underweight";
         
}
```
[Tip Calculator](https://www.codewars.com/kata/56598d8076ee7a0759000087/solutions/javascript)
```javascript
const TIPS = {
  "terrible": 0.0,
  "poor": 0.05,
  "good": 0.1,
  "great": 0.15,
  "excellent": 0.2
};

const calculateTip = (amount, rating) => {
  rating = rating.toLowerCase();
  
  return rating in TIPS ? Math.ceil(TIPS[rating] * amount) : "Rating not recognised";
};
// OR
function calculateTip(amount, rating) {
  let tip;
  rating = rating.toLowerCase(); 
  switch(rating) {
     case 'terrible':
      tip = amount * 0;
      break;
      
    case 'poor':
      tip = amount * 0.05;
      break;
      
    case 'good':
      tip = amount * 0.1;
      break;
      
    case 'great':
      tip = amount * 0.15;
      break;
      
    case 'excellent':
      tip = amount * 0.2;
      break;
    
    default:
      return 'Rating not recognised';
      break;
  }
  return Math.ceil(tip);
}
```
[The Office I - Outed](https://www.codewars.com/kata/57ecf6efc7fe13eb070000e1/solutions/javascript/me/best_practice)
```javascript
function outed(meet, boss){
let sum = meet[boss];
let a = 'Get Out Now!';
let b = 'Nice Work Champ!';
  for(let key in meet){
 sum += meet[key];
}
return (sum/Object.entries(meet).length <= 5) ? a : b
}
// OR
function outed(meet, boss) {
  let names = Object.keys(meet)
  let score = names.reduce((s,v) => s + meet[v], 0) + meet[boss]
  return score / names.length > 5 ? 'Nice Work Champ!' : 'Get Out Now!'
}
// OR
function outed(meet, boss){
  let total = Object.values(meet).reduce((t, v) => {
    return v + t}, meet[boss]);
  let overall = total / Object.keys(meet).length;
  return overall <= 5 ? "Get Out Now!" : "Nice Work Champ!"
}
```
[Regexp Basics - is it a digit?](https://www.codewars.com/kata/567bf4f7ee34510f69000032/solutions/javascript/me/best_practice)
```javascript
String.prototype.digit = function() {
  let arr = this.match(/[0-9]/g);
  
  if (!arr) return false;
  else if (this.length === arr.length && arr.length === 1) return true;
  else return false;
};
// OR
String.prototype.digit = function() {
  return /^\d$/.test(this);
};
```
[Keep up the hoop](https://www.codewars.com/kata/55cb632c1a5d7b3ad0000145/solutions/javascript/me/best_practice)
```javascript
function hoopCount(n) {
  return n >= 10 ?
    "Great, now move on to tricks" :
    "Keep at it until you get it";
}
// OR
function hoopCount (n) {
   return n > 9 ?
     "Great, now move on to tricks" :
     "Keep at it until you get it";
} 
```
[Simple Comparison?](https://www.codewars.com/kata/57f6ecdfcca6e045d2001207/solutions/javascript/me/best_practice)
```javascript

function add(a, b){
  return a == b 
}
// OR
const add = (a, b) => a == b

// 3rd SOLUT.

function add(a, b){
  return (`${a}`)==(`${b}`);
}

```
[To square(root) or not to square(root)](https://www.codewars.com/kata/57f6ad55cca6e045d2000627/solutions/javascript/me/best_practice)
```javascript
function squareOrSquareRoot(array) {
let arr = [];

for (let i = 0; i < array.length; i++){
if (Math.sqrt(array[i]) % 1 === 0 ){
  arr.push(Math.sqrt(array[i]))
}else
 arr.push(Math.pow(array[i],2))
}
return arr
}
// OR
function squareOrSquareRoot(array) {
  return array.map(function(num, i) { return Number.isInteger(Math.sqrt(num)) ? Math.sqrt(num) : num*num;});
}
```
[Remove the minimum](https://www.codewars.com/kata/563cf89eb4747c5fb100001b/solutions/javascript/me/best_practice)
```javascript
function removeSmallest(numbers) {
if(numbers.length === 0) return [];
  let arr = [];
  let min = numbers[0];
  for(let i = 1; i< numbers.length; i++){
     if(numbers[i] < min) min = numbers[i];
   }
 let index = numbers.indexOf(min);
 
  for(let i = 0; i< numbers.length; i++){
     if( i !== index) arr.push(numbers[i]);
  }
  return arr;
}
// OR 2nd SOLUTION.

function removeSmallest(numbers) {
  numbers = numbers.slice(0);
  const min = Math.min(...numbers);
  numbers.splice(numbers.indexOf(min), 1);
  return numbers;
}
```

