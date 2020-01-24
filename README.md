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

