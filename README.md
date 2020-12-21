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
[Invert values](https://www.codewars.com/kata/5899dc03bc95b1bf1b0000ad/solutions/javascript/me/best_practice)
```javascript
function invert(array) {
   return array.map(el => -el);
}
// 2ND SOLUTION
function invert(array) {
  var newArr = [];
  for(var i = 0; i < array.length; i++){
    newArr.push(-array[i]);
  }
   return newArr;
}
```
[Triple Trouble](https://www.codewars.com/kata/5704aea738428f4d30000914/solutions/javascript/me/best_practice)
```javascript
function tripleTrouble(one, two, three){
  let myStr = '';
  for(let i = 0; i < one.length; i++){
  myStr = myStr + one[i] + two[i] + three[i];
 }
 return myStr;
 }
// OR 2nd SOLUTION

function tripleTrouble(one, two, three){
  return one.replace(/./g,(v,i)=>v+two[i]+three[i])
 }
```
[Is he gonna survive?](https://www.codewars.com/kata/59ca8246d751df55cc00014c/solutions/javascript/me/best_practice)
```javascript
unction hero(bullets, dragons){
  return bullets >= dragons * 2
}
// OR 2ND SOL.

const hero = (bullets, dragons) => dragons * 2 <= bullets;
```
[Most valuable character](https://www.codewars.com/kata/5dd5128f16eced000e4c42ba/solutions/javascript/me/best_practice)
```javascript
function solve(st) {
 let max = 0;
 let obj = {}; 
 for(let i = 0; i < st.length; i++){
   obj[st[i]] = st.lastIndexOf(st[i]) - st.indexOf(st[i])
   if(obj[st[i]] > max) 
    max = obj[st[i]];
 }
 let min = 'Й';
 for(let key in obj){
   if( obj[key] === max && key < min) {
   min = key;
   }
 }
 return min
}
// 2ND SOLUTION
function solve(str) {
  let count = 0;
  let mvc = str[0];
     for(let s of str) {
      const diff = str.lastIndexOf(s) - str.indexOf(s)
       if(diff > count || diff === count && s.localeCompare(mvc) === -1) {
        count = diff;
        mvc = s;
       }
     }  
  return mvc;
}
```
[Take a Ten Minute Walk](https://www.codewars.com/kata/54da539698b8a2ad76000228/solutions/javascript)
```javascript
function isValidWalk(walk) {
   let s = 0, n = 0, w = 0, e = 0;
   for (let i = 0; i < walk.length; i++) {
     if (walk[i] === 's') s++;
     if (walk[i] === 'w') w++;
     if (walk[i] === 'n') n++;
     if (walk[i] === 'e') e++;
   }
   return s === n && w === e && walk.length === 10;;   
}
// OR 2ND SOLUTION
function isValidWalk(walk) {
  function count(val) {
    return walk.filter(function(a){return a==val;}).length;
  }
  return walk.length==10 && count('n')==count('s') && count('w')==count('e');
}
```
[Filling an array (part 1)](https://www.codewars.com/kata/571d42206414b103dc0006a1/solutions/javascript/me/best_practice)
```javascript
//const arr = N => [ /* the numbers 0 to N-1 */ ];
function arr(n) {
let a = [];
for(let i = 0; i <= n - 1; i++) {
  a.push(i);
}
return a;
}
// OR 2nd Solution

const arr = require('lodash').range;
```

[Find the first non-consecutive number](https://www.codewars.com/kata/58f8a3a27a5c28d92e000144/solutions/javascript/me/best_practice)
```javascript
function firstNonConsecutive (arr) {
 for(let i = 0; i < arr.length - 1; i++) {
  if(arr[i] + 1 !== arr[i + 1]) {
    return arr[i + 1];
    }
 }
  return null;
}
// OR 2ND SOLUTION
function firstNonConsecutive (arr) {
  for (let i=1; i<arr.length; i++) {
    if (arr[i] - arr[i-1] > 1) return arr[i]; 
  }
  return null;
}
```
[Difference of Volumes of Cuboids](https://www.codewars.com/kata/58cb43f4256836ed95000f97/solutions/javascript/me/best_practice)
```javascript
function findDifference(a, b) {
  let v1 = a[0] * a[1] * a[2];
  let v2 = b[0] * b[1] * b[2];
  
  return Math.abs(v1 - v2);
}
// OR 2ND SOLUTION

function findDifference(a, b) {
  return Math.abs(a.reduce((a,b)=>a*b) - b.reduce((a,b)=> a*b))
}
```
[Find the divisors!](https://www.codewars.com/kata/544aed4c4a30184e960010f4/solutions/javascript/me/best_practice)
```javascript
function divisors(int) {
  let a = [];
  for (let i = 2; i<int; i++){
   if (int % i === 0) a.push(i);
   }
   if (a.length === 0) return `${int} is prime`;
   else return a;
};
// OR 2ND SOLUTION

function divisors(x) {
  var result = [];
  for (var a = 2; a*a <= x; ++a) {
    if (x%a == 0) {
      var b = x/a;
      result.push(a);
      if (b != a) {
        result.push(b);
      }
    }
  }
  if (result.length == 0) {
    return x+' is prime';
  }
  result.sort(function (a, b) {
    return a - b;
  });
  return result;
};

// Interesting 3RD SOLUTION

function divisors(integer) {
  for(var div = [], i = 2; i < integer; i++) if(integer % i == 0) div.push(i);
  return div.length > 0 ? div : integer + " is prime";
}
```
[Grasshopper - Basic Function Fixer](https://www.codewars.com/kata/56200d610758762fb0000002/solutions/javascript/me/best_practice)
```javascript
function addFive(num) {
  num += 5;
  return num;
}
// OR 2ND SOLUTION

const addFive = (num) => num + 5

```
[Price of Mangoes](https://www.codewars.com/kata/57a77726bb9944d000000b06/solutions/javascript/me/best_practice)
```javascript
function mango(quantity, price){
  return (quantity - Math.floor(quantity/3))*price;
}
// 2ND SOLUTION

function mango(quantity, price){
  return (quantity - Math.floor(quantity/3))*price;
}
```
[Pre-FizzBuzz Workout #1](https://www.codewars.com/kata/569e09850a8e371ab200000b/solutions/javascript/me/best_practice)
```javascript
function preFizz(n) {
    let arr = [];

    for(let i = 1; i <= n; i++){
        arr.push(i);
    }

    return arr;
}
// OR 2ND SOLUTION

const preFizz = n => Array.from({length: n}, (_, i) => i + 1)
```
[Training JS #10: loop statement --for](https://www.codewars.com/kata/5721a78c283129e416000999/solutions/javascript/me/best_practice)
```javascript
function pickIt(arr) {
    let odd = [], even = [];
    for (let i = 0; i < arr.length; i++) {
        if (arr[i] % 2 === 0) {
            even.push(arr[i]);
        } else {
            odd.push(arr[i]);
        }
    }
    return [odd, even];
}
// OR 2ND SOLUTION

function pickIt(arr){
  var odd=[],even=[]
  //coding here
  for (var i=0;i<arr.length;i++){
    if (arr[i]%2==1) odd.push(arr[i]);
    else            even.push(arr[i]);
  }
  return [odd,even];
}
```
[isReallyNaN](https://www.codewars.com/kata/56c24c58e0c0f741d4001aef/solutions/javascript/me/best_practice)
```javascript
const isReallyNaN = (val) => {
  
  return Number.isNaN(val);
};
// OR 2ND SOLUTION

const isReallyNaN = Number.isNaN

```
[Is it a palindrome?](https://www.codewars.com/kata/57a1fd2ce298a731b20006a4/solutions/javascript/me/best_practice)
```javascript
function isPalindrome(x) {
  let reverse = '';
  x = x.toLowerCase();
  for (let i = x.length - 1; i >= 0; --i) {
    reverse += x[i]
  }
  return x == reverse;
}
// OR 2ND SOLUTION

function isPalindrome(x) {
  return x.toLowerCase()==x.split('').reverse().join('').toLowerCase()
}
```
[Removing Elements](https://www.codewars.com/kata/5769b3802ae6f8e4890009d2/solutions/javascript/me/best_practice)
```js
function removeEveryOther(arr){
  let arr2 = [];
  for (let i = 0; i < arr.length; i += 2) {
    arr2.push(arr[i]);
  }
  return arr2;
}
//  OR  2ND SOLUTION

function removeEveryOther(arr){
  return arr.filter(function(elem, index) {
    return index % 2 === 0;
  });
};
```

[Row Weights](https://www.codewars.com/kata/5abd66a5ccfd1130b30000a9/solutions/javascript/me/best_practice)
```js
function rowWeights(arr){
  let sumOddIndex = 0;
  let sumEvenIndex = 0;
   for (let i = 0; i < arr.length; ++i) {
    if (i % 2 !== 0) {
  sumEvenIndex += arr[i]
   } else {
  sumOddIndex += arr[i]
   }
  }
return [sumOddIndex, sumEvenIndex]
};
//  OR 2ND SOLUTION

function rowWeights(arr){
  let sumTeam1 = 0;
  let sumTeam2 = 0;
  for (i = 0; i < arr.length; i++){
    if (i % 2 === 0) sumTeam1 = sumTeam1 + arr[i];
      else sumTeam2 = sumTeam2 + arr[i];
  }
  return [sumTeam1, sumTeam2];
}

```
[Take a Ten Minute Walk](https://www.codewars.com/kata/54da539698b8a2ad76000228/solutions/javascript)
```js
function isValidWalk(walk) {
  var dx = 0
  var dy = 0
  var dt = walk.length
  
  for (var i = 0; i < walk.length; i++) {
    switch (walk[i]) {
      case 'n': dy--; break;
      case 's': dy++; break;
      case 'w': dx--; break;
      case 'e': dx++; break;
    }
  }
  
  return dt === 10 && dx === 0 && dy === 0
};

//  OR 2ND SOLUTION.

function isValidWalk(walk) {
  let total = 0;
  if(walk.length!==10) return false;
  for(el of walk)
    el==='n' || el==='w' ? total++ : total--;
  return !total;
}
```

[Find the middle element](https://www.codewars.com/kata/545a4c5a61aa4c6916000755/solutions/javascript/me/best_practice)
```js

function gimme(arr) {
  let max = Math.max(...arr)
  let min = Math.min(...arr);
  for(let i = 0; i < arr.length; i++){
    if(arr[i] !== max && arr[i] !== min){
    return i;
    }
  }
}
// OR  2ND Solution.

var gimme = function (inputArray) {
 var order = inputArray.slice().sort(function(a,b) { return a-b;});
 return inputArray.indexOf(order[1]);
  
};

```
[Multiplication table](https://www.codewars.com/kata/534d2f5b5371ecf8d2000a08/solutions/javascript/me/best_practice)
```js
multiplicationTable = function(size) {
  const arr = [];
  
  for (let i = 1; i <= size;i++) {
    const newArr = [];
    arr.push(newArr);
    for (let j = 1; j <= size; j++) {
      newArr.push(i * j)
    }
  }
  return arr;
}

//  OR 2ND SOLUTION.

multiplicationTable = function(size) {
  var table = [];
  for (i = 1; i <= size; i++){
    var row = [];
    for (j = 1; j <= size; j++) row.push(i * j);
      table.push(row);
    }
  return table;
}
```
[Filter out the geese](https://www.codewars.com/kata/57ee4a67108d3fd9eb0000e7/solutions/javascript/me/best_practice)
```js
function gooseFilter (birds) {
  var geese = ["African", "Roman Tufted", "Toulouse", "Pilgrim", "Steinbacher"];
  const noGeese = [];
   for (let i = 0; i < birds.length; i++){
     if(!geese.includes(birds[i]))
     noGeese.push(birds[i]);
     }
     return noGeese;
} 

// OR 2ND SOLUTION.

const geese = ["African", "Roman Tufted", "Toulouse", "Pilgrim", "Steinbacher"]

const notGoose = bird =>
  !geese.includes(bird)

const gooseFilter = birds =>
  birds.filter(notGoose)

```
[Sorted? yes? no? how?](https://www.codewars.com/kata/580a4734d6df748060000045/solutions/javascript/me/best_practice)
```js
function isSortedAndHow(arr) {
let res = 0;
let n = 0;
for(let i = 0; i<arr.length; i++) {
if(arr[i] < arr[i+1]) 
res++;
else if (arr[i] > arr[i+1])
n++;
}
if(res > 0 && n === 0) return "yes, ascending";
else if(res === 0 && n > 0) return "yes, descending";
else return "no";
};

//  OR 2ND SOLUTION.

function isSortedAndHow(arr) {
  return arr.every((x,i)=>i==0||arr[i]>=arr[i-1])?'yes, ascending':
         arr.every((x,i)=>i==0||arr[i]<=arr[i-1])?'yes, descending':'no'
}
```
[Moving Zeros To The End](https://www.codewars.com/kata/52597aa56021e91c93000cb0/solutions/javascript/me/best_practice)
```js
var moveZeros = function (arr) {
  const arr1 = [];
  let count = 0;
  for(let i = 0; i < arr.length; ++i){
    if(arr[i] !== 0) arr1.push(arr[i]);
    else count++;
  }
  for(let i = 0; i < count; ++i){
  
  arr1.push(0)
  }
 return arr1;
};
//  OR 2nd SOLUTION.

var moveZeros = function (arr) {
  for(var i = arr.length - 1; i >= 0; i--) {
    if(arr[i] === 0) {
      arr.splice(i, 1);
      arr.push(0);
    }
  }
  return arr;
}
```

[Get Planet Name By ID](https://www.codewars.com/kata/515e188a311df01cba000003/solutions/javascript/me/best_practice)
```js
function getPlanetName(id){
  let obj = {
   1: 'Mercury',
   2: 'Venus',
   3: 'Earth',
   4: 'Mars',
   5: 'Jupiter',
   6: 'Saturn',
   7: 'Uranus',
   8: 'Neptune',
  }
  
  return obj[id];
};

//  OR 2ND SOLUTION.

function getPlanetName(id){
  switch(id){
    case 1:
      return 'Mercury'
    case 2:
      return 'Venus'
    case 3:
      return 'Earth'
    case 4:
      return 'Mars'
    case 5:
      return 'Jupiter'
    case 6:
      return 'Saturn'
    case 7:
      return 'Uranus'
    case 8:
      return 'Neptune'
  }

}
```
[Welcome!](https://www.codewars.com/kata/577ff15ad648a14b780000e7/solutions/javascript/me/best_practice)
```js
function greet(l) {
  return {
    english: 'Welcome',
    IP_ADDRESS_INVALID: 'Welcome',
    IP_ADDRESS_NOT_FOUND: 'Welcome',
    IP_ADDRESS_REQUIRED: 'Welcome',
    czech: 'Vitejte',
    danish: 'Velkomst',
    dutch: 'Welkom',
    estonian: 'Tere tulemast',
    finnish: 'Tervetuloa',
    flemish: 'Welgekomen',
    french: 'Bienvenue',
    german: 'Willkommen',
    irish: 'Failte',
    italian: 'Benvenuto',
    latvian: 'Gaidits',
    lithuanian: 'Laukiamas',
    polish: 'Witamy',
    spanish: 'Bienvenido',
    swedish: 'Valkommen',
    welsh: 'Croeso'
  }[l];
};

//  OR 2ND SOLUTION.

var database = {
english: 'Welcome',
czech: 'Vitejte',
danish: 'Velkomst',
dutch: 'Welkom',
estonian: 'Tere tulemast',
finnish: 'Tervetuloa',
flemish: 'Welgekomen',
french: 'Bienvenue',
german: 'Willkommen',
irish: 'Failte',
italian: 'Benvenuto',
latvian: 'Gaidits',
lithuanian: 'Laukiamas',
polish: 'Witamy',
spanish: 'Bienvenido',
swedish: 'Valkommen',
welsh: 'Croeso'
}

function greet(language) {
return database[language] || "Welcome";
}

```
[Rock Paper Scissors!](https://www.codewars.com/kata/5672a98bdbdd995fad00000f/solutions/javascript/me/best_practice)
```js
const rps = (p1, p2) => {
let message1 = 'scissors';
let message2 = 'rock';
let message3 = 'paper';
if (p1 === message1 && p2 === message1) return 'Draw!';
if (p1 === message2 && p2 === message2) return 'Draw!';
if (p1 === message3 && p2 === message3) return 'Draw!';
if (p1 === message1 && p2 === message2) return 'Player 2 won!';
if (p1 === message1 && p2 === message3) return 'Player 1 won!';
if (p1 === message2 && p2 === message1) return 'Player 1 won!';
if (p1 === message2 && p2 === message3) return 'Player 2 won!';
if (p1 === message3 && p2 === message1) return 'Player 2 won!';
if (p1 === message3 && p2 === message2) return 'Player 1 won!';
}

// AND/OR 2ND SOLUTION.

const rps = (p1, p2) => {
  if (p1 == p2)
    return 'Draw!';
    
   if (p1 == 'rock' && p2 == 'scissors') 
     return 'Player 1 won!'
   else if (p1 == 'scissors' && p2 == 'paper') 
     return 'Player 1 won!'
   else if (p1 == 'paper' && p2 == 'rock') 
     return 'Player 1 won!'
   else
     return 'Player 2 won!';
};
```
[Rock Paper Scissors Lizard Spock](https://www.codewars.com/kata/57d29ccda56edb4187000052/solutions/javascript/me/best_practice)
```js
function rpsls(pl1,pl2){
let arr = [ "Scissors Paper", 
"Paper Rock",
"Rock Lizard",
"Lizard Spock",
"Spock Scissors",
"Scissors Lizard",
"Lizard Paper",
"Paper Spock",
"Spock Rock",
"Rock Scissors"]
arr = arr.map(el=> el.toLowerCase());
let str = pl1 + ' ' +pl2;
if (arr.includes(str)) return "Player 1 Won!";
else if (pl1 === pl2) return "Draw!";
else return "Player 2 Won!"
return str;

}

// OR 2ND SOLUTION.

function rpsls(pl1, pl2){
  const moves = ['scissors', 'paper', 'rock', 'lizard', 'spock'];
  const winner = (5 + moves.indexOf(pl2) - moves.indexOf(pl1)) % 5;
  
  return winner ? `Player ${winner % 2 ? 1 : 2} Won!` : 'Draw!';
}
```
[Find the Capitals](https://www.codewars.com/kata/53573877d5493b4d6e00050c/solutions/javascript/me/best_practice)
```
function capital(capitals){
  const arr = [];
  for (let i = 0; i < capitals.length; i++) {
    if (capitals[i].hasOwnProperty('state')){
      arr.push(`The capital of ${capitals[i]['state']} is ${capitals[i]['capital']}`);
    }
    if (capitals[i].hasOwnProperty('country')){
      arr.push(`The capital of ${capitals[i]['country']} is ${capitals[i]['capital']}`);
   }
  }
  return arr;
}
//  OR 2ND SOLUTION.

function capital(capitals){
  return capitals.map(function(o){
    return "The capital of " + (o.state || o.country) + " is " + o.capital;
  });
}

```
[Test's results](https://www.codewars.com/kata/599db0a227ca9f294b0000c8/solutions/javascript/me/best_practice)
```
function testResult(array) {
  let sum = 0;
  for(let i = 0; i < array.length; i++){
  sum += array[i];
  }
  let sumAvr = +(sum / array.length).toFixed(3);
  let obj = {
    'h': 0,
    'a': 0,
    'l': 0,
    }
    for (let el of array){
    if(el >= 9) obj['h']++
    else if(el >= 7) obj['a']++
    else obj['l']++
    }
    return (obj['a'] + obj['l'] === 0) ? [sumAvr, obj, 'They did well'] : [sumAvr, obj];
}

//  OR 2ND SOLUTION.

function testResult(array) {
let count = 0;
let obj = {'h': 0, 'a': 0, 'l': 0};
let arr = [];
for( let i in array) {
count += array[i];
if (array[i] > 8) obj['h'] ++;
else if (array[i] > 6) obj['a'] ++;
else obj['l'] ++;
} return (obj['a'] == 0 && obj['l'] == 0)?
[+(count/array.length).toFixed(3), obj,'They did well']:
[+(count/array.length).toFixed(3), obj];
};

```
[Rock Off!](https://www.codewars.com/kata/5b097da6c3323ac067000036/solutions/javascript/me/best_practice)
```
function solve(a, b) {
  let sumA = 0;
  let sumB = 0;
  for ( let i = 0; i < 3; i++ ) {
    if ( a[i] > b[i]) sumA++
    else if ( a[i] < b[i]) sumB++
  }
  if (sumA > sumB) return `${sumA}, ${sumB}: Alice made "Kurt" proud!`
  else if (sumA < sumB) return  `${sumA}, ${sumB}: Bob made "Jeff" proud!`
  else return  `${sumA}, ${sumB}: that looks like a "draw"! Rock on!`
  
};

// OR 2ND SOLUTION.

function solve(a, b) {

let scoreA = 0;
let scoreB = 0;  

for (let i = 0; i < 3; i++ ){
if (a[i] > b[i]) scoreA +=1; 
if (a[i] < b[i]) scoreB +=1; 
  
  }
if (scoreA > scoreB) return `${scoreA}, ${scoreB}: Alice made "Kurt" proud!`; 
if (scoreA < scoreB) return `${scoreA}, ${scoreB}: Bob made "Jeff" proud!`; 
if (scoreA === scoreB) return `${scoreA}, ${scoreB}: that looks like a "draw"! Rock on!`;   
};

```
[Bumps in the Road](https://www.codewars.com/kata/57ed30dde7728215300005fa/solutions/javascript/me/best_practice)
```
function bump(x){
  let count = 0;
  for(let i = 0;i<=x.length;i++){
if(x[i]==='n'){
  count++
}
}if(count>15){
  return "Car Dead"
}else{
  return "Woohoo!"
}
  };

//  OR/AND 2ND SOLUTION.

const bump = x =>
  --x.split(`n`).length > 15 ? `Car Dead` : `Woohoo!`;

```

[Credit Card Mask](https://www.codewars.com/kata/5412509bd436bd33920011bc/solutions/javascript/me/best_practice)
```
function maskify(cc) {
let a = '';
  for (let i = 0; i < cc.length; i++)
    {if(i<cc.length-4) {a+='#'}
  else a+=cc[i];}
  return a;
};

// OR 2ND SOLUTION.

function maskify(cc) {
  return cc.slice(0, -4).replace(/./g, '#') + cc.slice(-4);
};

```
[Spacify](https://www.codewars.com/kata/57f8ee485cae443c4d000127/solutions/javascript/me/best_practice)
```
function spacify(str) {
  let nStr = '';
  for(let i = 0; i<str.length-1; i++){nStr += str[i]+' '}
  return nStr + str[str.length-1];
};

// OR 2ND SOLUTION.

const spacify = str => [...str].join(' ');

```

[Reversed Strings](https://www.codewars.com/kata/5168bb5dfe9a00b126000018/solutions/javascript/me/best_practice)
```
function solution(str) {
  let newStr = '';
  for(let i = str.length - 1; i >= 0; i--)  {
    newStr += str[i];
  }
  return newStr;
};

// OR 2ND SOLUTION.

const solution = s => [...s].reverse().join('')

// AND 3RD SOLUTION.

function solution(str){
  return str.split('').reverse().join('');  
};

```

[Factorial](https://www.codewars.com/kata/57a049e253ba33ac5e000212/solutions/javascript/me/best_practice)
```
function factorial(n){
 let num = 1;
  let product = 1;
  while(num <= n){
    product = product * num;
    num++;
  }
  return product;
};

// OR 2ND SOLUTION.

const factorial = n => n <= 0 ? 1 : n * factorial(n - 1);

```

[Powers of 3](https://www.codewars.com/kata/57be674b93687de78c0001d9/solutions/javascript/me/best_practice)
```
function largestPower(n){
  let k = 0;
    for ( k = 0; 3**k < n; k++) {
      
    }
  return k-1;
};

//  OR 2ND SOLUTION.

function largestPower(n){
  if (n == 3 || n == 2 || n == 0) {
      return 0;
  }
  else if (n == 1) {
      return -1;
  }
  else {
      return Math.trunc(Math.log(n-1)/Math.log(3));
  }
};

```

[Breaking chocolate problem](https://www.codewars.com/kata/534ea96ebb17181947000ada/solutions/javascript/me/best_practice)
```
function breakChocolate(n,m) {
 if( (n+m)>2 && n>0 && m>0 ) {
   return (n*m-1);
 }
 else {
  return 0;
 }
};

// OR 2ND SOLUTION.

function breakChocolate(n,m) {
 if(n === 0 || m === 0) return 0
 return n * m - 1;
};

```

[Miles per gallon to kilometers per liter](https://www.codewars.com/kata/557b5e0bddf29d861400005d/solutions/javascript/me/best_practice)
```
function converter (mpg) {
  let kil = 1.609344;
  let lit = 4.54609188
  let kpl = mpg * kil / lit;
  return parseFloat(kpl.toFixed(2));
};

// OR 2ND SOLUTION.

function converter (mpg) {
  return +(mpg * .354006043538).toFixed(2)
};

 // AND 3RD SOLUTION.

function converter (mpg) {
  return Math.round( mpg * 160.9344 / 4.54609188 ) / 100
};

```

[Counting sheep...](https://www.codewars.com/kata/54edbc7200b811e956000556/solutions/javascript/me/best_practice)
```
function countSheeps(arr) {
  let count = 0;

  for (let i = 0; i < arr.length; i++) {
    if (arr[i] === true) {
      count++;
    }
  }

  return count;
};

// OR 2ND SOLUTION.

function countSheeps(arr) {
  return arr.filter(Boolean).length;
};

```

[Sum of positive](https://www.codewars.com/kata/5715eaedb436cf5606000381/solutions/javascript/me/best_practice)
```
function positiveSum(arr) {
  let sum=0
  for(let el of arr){
    if (el>0){sum =sum+el} }
return sum
};

// OR 2ND SOLUTION.

function positiveSum(arr) {
  let sum = 0;
  
  for (n of arr) {
    if (n > 0) sum += n;
  }
  
  return sum;
};

```

[Simple Fun #152: Invite More Women?](https://www.codewars.com/kata/58acfe4ae0201e1708000075/solutions/javascript/me/best_practice)
```

function inviteMoreWomen(L) {
  let sum=0
  for(let i = 0; i<L.length; i++){
    sum+=L[i];
  }  
  if(sum>0) return true;
  if(sum<=0) return false;
};

// OR 2ND SOLUTION.

function inviteMoreWomen(L) {
  return L.reduce((a,b) => a+b) > 0;
}

```

[Filter the number](https://www.codewars.com/kata/55b051fac50a3292a9000025/solutions/javascript/me/best_practice)
```
var FilterString = function(value) {

let str = value;
let num = '';
  for(let i = 0; i < str.length; i++){
    if(isNaN(str[i]) == false) 
    num += str[i];
    }
    return + num;
  };

// 2ND SOLUTION.

function FilterString(value) {
  return Number(value.replace(/[^\d]/g, ""))
}

```

[Basic Training: Add item to an Array](https://www.codewars.com/kata/511f0fe64ae8683297000001/solutions/javascript/me/best_practice)
```
// add the value "codewars" to the already defined websites array
websites.push('codewars')

// OR 2ND SOL.

// add the value "codewars" to the already defined websit
websites[0]="codewars";

```

[Sum Arrays](https://www.codewars.com/kata/53dc54212259ed3d4f00071c/solutions/javascript/me/best_practice)
```
// Sum Numbers
function sum (numbers) {
    "use strict";
    let sumNum = 0;
    for(let i = 0; i< numbers.length; i++){
      sumNum+=numbers[i];
    } return sumNum;
    
};

// OR 2ND SOLUTION.

function sum(numbers) {
  return numbers.reduce((a, b) => a + b, 0);
};

```

[Sum even numbers](https://www.codewars.com/kata/586beb5ba44cfc44ed0006c3/solutions/javascript/me/best_practice)
```
function sumEvenNumbers(input) {
  let num = 0;
  for(let i = 0; i<input.length; i++){
    if(input[i] % 2 === 0){
      num += input[i];
    }
    
  }
  return num;
  // [...]
}

// OR 2ND SOLUTION.

function sumEvenNumbers(input) {
  let sum = 0;
  for(let elm of input){
      if(elm %2 === 0){
          sum = sum + elm;
      }
  }
  return sum;
}

```

[Find the Slope](https://www.codewars.com/kata/55a75e2d0803fea18f00009d/solutions/javascript/me/best_practice)
```
function slope(points)
{
  let deltaX = points[3] - points[1];
  let deltaY = points[2] - points[0];
  return (deltaY === 0)? 'undefined': `${deltaX / deltaY}`;
};

// OR 2ND SOLUTION.

function slope(points) {
  let dx = points[2] - points[0],
      dy = points[3] - points[1]
      
  if (dx == 0)
    return 'undefined'
  
  return (dy/dx) + ''
}

```
[Generate range of integers](https://www.codewars.com/kata/55eca815d0d20962e1000106/solutions/javascript/me/best_practice)
```
function generateRange(min, max, step){
  let arr = [];
  for (let x = min ; x <= max ; x += step)
    arr.push(x);
  return arr;
}

// OR 2ND SOLUTION.

function generateRange(min, max, step){
  var arr = [];
  while (min <= max) {
    arr.push(min);
    min += step;
  }
  return arr
}
```

[Coefficients of the Quadratic Equation](https://www.codewars.com/kata/5d59576768ba810001f1f8d6/solutions/javascript/me/best_practice)
```
function quadratic(x1, x2) {
  return [1, -(x1 + x2), x1 * x2];
}

// OR 2ND SOLUTION.

const quadratic = (x1, x2) => [
  1,
  -x1 -x2,
  x1 * x2
]

```
[Squares sequence](https://www.codewars.com/kata/5546180ca783b6d2d5000062/solutions/javascript/me/best_practice)
```
function squares(x, n) {
  let arr = [];
  for (let i = 0; i < n; i++) {
    arr.push(x);
    x = x ** 2;
  } return arr;
};

// OR 2ND SOLUTION.

function squares(x, n) {
  const arr = [];
    for (let i = x; arr.length < n; i = i ** 2) {
      arr.push(i);
  }
  return arr
};

```
[For Twins: 2. Math operations](https://www.codewars.com/kata/59c287b16bddd291c700009a/solutions/javascript/me/best_practice)
```
function iceBrickVolume(radius, bottleLength, rimLength) {
  let h = bottleLength - rimLength;
  let s = 2 * radius ** 2;
  let v = h * s;
  return v
}

// OR 2ND SOLUTION.

const iceBrickVolume = (r, x, y) => 2 * r * r * (x - y);

```
[I love you, a little , a lot, passionately ... not at all](https://www.codewars.com/kata/57f24e6a18e9fad8eb000296/solutions/javascript/me/best_practice)
```
function howMuchILoveYou(nbPetals) {
    // your code
    let phrases = ["not at all","I love you","a little","a lot","passionately","madly"];
    return phrases[(nbPetals%6) ];
}

// OR 2ND SOLUTION.

function howMuchILoveYou(nbPetals) {
  let phrase = {    
    0: "not at all",
    1: "I love you",
    2: "a little",
    3: "a lot",
    4: "passionately",
    5: "madly"
  }
  return phrase[nbPetals%6]
}
```
[Function 3 - multiplying two numbers](https://www.codewars.com/kata/523b66342d0c301ae400003b/solutions/javascript/me/best_practice)
```
function multiply( a, b ){
  return a * b;
}

// OR 2ND SOLUTION.

function multiply(a, b){
  if(typeof a == 'number' && typeof b == 'number')
    return a * b;  
}
```

[Grasshopper - Messi Goals](https://www.codewars.com/kata/55ca77fa094a2af31f00002a/solutions/javascript/me/best_practice)
```
var laLigaGoals = 43
var championsLeagueGoals = 10
var copaDelReyGoals = 5

var totalGoals = laLigaGoals + championsLeagueGoals + copaDelReyGoals

//OR 2ND SOLUTION.

var laLigaGoals = 43
var championsLeagueGoals = 10
var copaDelReyGoals = 5

function sum(...num) {
  let ad = 0;
  num.forEach( e => {
    ad+=e
  })
  return ad            
}

var totalGoals = sum(laLigaGoals, championsLeagueGoals, copaDelReyGoals)
```

[Count Odd Numbers below n](https://www.codewars.com/kata/59342039eb450e39970000a6/solutions/javascript/me/best_practice)
```
function oddCount(n){
  return Math.floor(n/2);
}

// OR 2ND SOLUTION.

const oddCount = n => Math.floor(n/2) ;
```

[My head is at the wrong end!](https://www.codewars.com/kata/56f699cd9400f5b7d8000b55/solutions/javascript/me/best_practice)
```
function fixTheMeerkat(arr) {
  return arr.reverse();
}
// OR 2ND SOLUTION.

function fixTheMeerkat(arr) {
  return [arr[2], arr[1], arr[0]];
}
```

[Convert number to reversed array of digits](https://www.codewars.com/kata/5583090cbe83f4fd8c000051/solutions/javascript/me/best_practice)
```
function digitize(n) {
  n = n + '';
  return n.split('').reverse().map(el => + el);
  console.log(arr);
};
// OR/AND 2ND SOLUTION.

function digitize(n) {
  return n.toString().split("").reverse().map(function(i){
    return parseInt(i);
  });
}
```

[The Skiponacci Sequence](https://www.codewars.com/kata/580777ee2e14accd9f000165/solutions/javascript/me/best_practice)
```
function skiponacci(n) {
  if (n === 1) return '1';
  let fib = [1, 1];
  for (let i = 2; i < n; i++){
    fib.push(fib[i-1] + fib[i-2]);
  }
  return fib.map((el, i) => i % 2 !== 0? 'skip' : el).join(' ');
}
// OR/AND 2ND SOLUTION.

function skiponacci(n) {
  if (n === 1) return '1';
let fib = [1, 1];
  for (let i = 2; i < n; i++){
    fib.push(fib[i-1] + fib[i - 2])
  }
  return arr = fib.map((el, i) => i % 2 !== 0? 'skip' : el).join(' ')
}
```

[Take an Arrow to the knee, Functionally](https://www.codewars.com/kata/559f3123e66a7204f000009f/solutions/javascript/me/best_practice)
```
var ArrowFunc = function(arr) {
  return arr.map(el => String.fromCharCode(el)).join(''); //Complete this function
}
// OR 2ND SOLUTION.

const ArrowFunc = (arr) => arr.map(c => String.fromCharCode(c)).join("")

```
[No Loops 2 - You only need one](https://www.codewars.com/kata/57cc40b2f8392dbf2a0003ce/solutions/javascript/me/best_practice)
```
function check(a, x) {
  return a.includes(x);
}
// OR/AND 2ND SOLUTION.

const check = (a,x) => a.includes(x);
```
[You only need one - Beginner](https://www.codewars.com/kata/57cc975ed542d3148f00015b/solutions/javascript/me/best_practice)
```
function check(a,x){
  return a.includes(x);
};
// OR/AND 2ND SOLUTION.

function check(a,x){
  return a.indexOf(x) > -1 ? true : false;
};

```
[JavaScript Array Filter](https://www.codewars.com/kata/514a6336889283a3d2000001/solutions/javascript/me/best_practice)
```
function getEvenNumbers(numbersArray){
  return numbersArray.filter(el => el % 2 === 0);
}
// OR/AND 2ND SOLUTION.

function getEvenNumbers(numbersArray){
  return numbersArray.filter(function(n){
    return n % 2 == 0;
  });
}
```
[filterEvenLengthWords](https://www.codewars.com/kata/59564f3bcc15b5591a00004a/solutions/javascript/me/best_practice)
```
function filterEvenLengthWords(words) {
  return words.filter(el => el.length % 2 === 0);
}
// OR/AND 2ND SOLUTION.

function filterEvenLengthWords(words){
  //let count = 0;
  let arr = [];
  for(let i = 0; i < words.length; i++){
    if(words[i].length % 2 == 0){
      arr.push(words[i]);
      //count++;
    }
  }
  //return [count];
  return arr;
}
```
[Find the lucky numbers](https://www.codewars.com/kata/580435ab150cca22650001fb/solutions/javascript/me/best_practice)
```
var filterLucky=x=>{
  return x.filter(el => String(el).split('').includes('7'));
}
// OR 2ND SOLUTION.

function filterLucky(arr) {
  return arr.filter((elem) => elem.toString().includes('7'));
}
```

[List Filtering](https://www.codewars.com/kata/53dbd5315a3c69eed20002dd/solutions/javascript/me/best_practice)
```
function filter_list(l) {
  return l.filter((el) => typeof el === 'number' );
}
OR 2ND SOLUTION.

function filter_list(l) {
 return l.filter(v => typeof v == "number")
}
```

[Array.diff](https://www.codewars.com/kata/523f5d21c841566fde000009/solutions/javascript/me/best_practice)
```
function arrayDiff(a, b) {
  return a.filter( ( el ) => !b.includes( el ) );
}
// OR/AND 2ND SOLUTION.

array_diff = require("lodash").difference;
```

[Return the closest number multiple of 10](https://www.codewars.com/kata/58249d08b81f70a2fc0001a4/solutions/javascript/me/best_practice)
```
const closestMultiple10 = num => {
  return Math.round(num/10)*10;
};
// OR/AND 2ND SOLUTION.

function closestMultiple10 (num) {
  let x = num % 10;
  let y = num - x;
  return x >= 5 ? y + 10 : y;
}
```

[Two Oldest Ages](https://www.codewars.com/kata/511f11d355fe575d2c000001/solutions/javascript/me/best_practice)
```
function twoOldestAges(ages){
  ages = ages.sort((a, b) => b - a);
  return [ages[1], ages[0]];
}
// OR/AND 2ND SOLUTION.

function twoOldestAges(ages){
  return ages.sort(function(a,b){return a-b;}).slice(-2);
}
```

[Simple frequency sort](https://www.codewars.com/kata/5a8d2bf60025e9163c0000bc/solutions/javascript/me/best_practice)
```
function solve(arr){
  let obj = {};
  for (let el of arr){
    if (obj[el]) obj[el]++;
    else obj[el] = 1;
  }
  arr = arr.sort((a, b) => obj[b] === obj[a] ? a - b : obj[b] - obj[a]);
  return arr;
}
// OR 2ND SOLUTION.

function solve(arr){
  
    console.log(arr)

    // Сортируем массив по значениям
    let sorted = []
    sorted = arr.sort(function(a,b){
        return a-b
    })

  
    // Создаем 2d массив с элементом и количестов появлений
    let sorted_2d = []
    while (sorted.length){
        let item = sorted.shift()
        let count = 1
        for(let i of sorted){
            if (item === i) {
                count += 1
            }
        }
        sorted = sorted.filter(function(x){
            return x != item
        })
        sorted_2d.push([item, count])
    }
 
    console.log('перед сортировкой', sorted_2d)
    // Сортируем 2д массив по количеству появлений
    sorted_2d = sorted_2d.sort(function(a,b){
        if (a[1] === b[1]) {
            return a[0]-b[0]
        }
        return b[1] - a[1]
    })
    console.log('после сортировки', sorted_2d)


    // Создаем финальный массив
    let final = []
    for (let i of sorted_2d) {
        let elem = i[0]
        let elem_count = i[1]
        let count = 1
        while (count <= elem_count) {
            final.push(elem)
            count += 1
        }
    }
  
  console.log(final)
    return final
}
```

[Be Concise I - The Ternary Operator](https://www.codewars.com/kata/56f3f6a82010832b02000f38/solutions/javascript/me/best_practice)
```
// TODO: Refactor and shorten the function

function describeAge(a) {
  return `You're a(n) ${a<= 12?"kid":a>=13&&a<=17?"teenager":a>=18&&a<=64?"adult":"elderly"}`
}
// OR 2ND SOLUTION.

function describeAge(a) {    
  return "You're a(n) " + (
    a > 64 ? "elderly":
      a > 17 ? "adult":
        a > 12 ? "teenager":
          "kid"
    );
}
// AND 3RD SOLUTION.

describeAge=a=>
`You're a(n) ${a
<13?'kid':a<18?
'teenager':a<65?
'adult':'elderly'}`

```

[Training JS #29: methods of arrayObject---concat() and join()](https://www.codewars.com/kata/5731861d05d14d6f50000626/solutions/javascript/me/best_practice)
```
function bigToSmall(arr){
 let res = [];
  
  for (let el of arr) {
    res = res.concat(el);
    
  }
  return res.sort((a, b) => b - a).join('>');
}
// OR 2ND SOLUTION.

function bigToSmall(arr){
 let newArr = [].concat(...arr);
let newArr1 = newArr.sort((a, b) => b - a).join('>')
return newArr1

}
```

[Round up to the next multiple of 5](https://www.codewars.com/kata/55d1d6d5955ec6365400006d/solutions/javascript/me/best_practice)
```
function roundToNext5(n){
  while(n % 5 !== 0) n++;
  return n;
}
// OR 2ND SOLUTION.

function roundToNext5(n){
  return Math.ceil(n/5)*5;
}
// Also interesting Solution.

roundToNext5=a=>Math.ceil(a/5)*5
```

[Power](https://www.codewars.com/kata/562926c855ca9fdc4800005b/solutions/javascript/me/best_practice)
```
function numberToPower(number, power){
  let p_0 = 1;
  for (let i = 1; i <= power; i++) {
    p_0 *= number;
  }
  return p_0;
}
// OR 2ND SOLUTION.

function numberToPower(number, power){
  var total = 1;
  for (var i = 1; i <= power; i++) { 
    total = total * number;
  }
  return total;
}
```

[You're a square!](https://www.codewars.com/kata/54c27a33fb7da0db0100040e/solutions/javascript/me/best_practice)
```
var isSquare = function(n){
  return Math.sqrt(n)%1===0
}
// OR 2ND SOLUTION.

const isSquare = n => Number.isInteger(Math.sqrt(n));

// AND 3RD SOLUTION.

var isSquare = function(n){

  if((Math.sqrt(n) % 1) == 0)
    return true;
  else
    return false;
}
```

[]






















































