# solvedTasks
# My wi-fi doesn't allow me to download the Git for 3-4 time. I will update repository from gitHub.
# JS Practise: Section 2.2 (solved around 8 CW tasks).
# 11-Dec-2019. JS Practise. Reached 2-3 + LEcture with Vladimir.
# 12-Dec-2019. Java Class with Sergey. JSP. Installed and set up Git

Convert a String to a Number!
```javascript
let stringToNumber = function(str){
  return Number(str);
}
```
Sum The Strings
```javascript
function sumStr(a,b) {
  a=+a;
  b=+b;
  return String(a+b);
}
```
Century From Year (codewars)
```javascript
function century(year) {
  let div=year/100;
  for (let i=1; i<=Math.ceil(year/100); i++){
  if (div<=i) {
    return 1
  } else if (div>i && div<=i+1){
    return i+1;
    }
    }
    }
```
Count Odd numbers below n
```javascript
function oddCount(n) {
     return Math.floor(n/2);
}
```
Return the closest number multiple of 10
```javascript
const closestMultiple10 = num => {
if (num<10) {
return 10
} else {
return Math.round(num/10)*10;
}
}
```
Area of a Square
```javascript
function squareArea(A){
  return +Math.pow((4*A)/(2*Math.PI),2).toFixed(2);
}
```
Formatting decimal places #0
```javascript
function twoDecimalPlaces(n) {
  return +n.toFixed(2);
}
```
Discover The Original Price
```javascript
function discoverOriginalPrice(discountedPrice, salePercentage){
  return +((discountedPrice*100)/(100-salePercentage)).toFixed(2);
}
```


