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
Simple Comparison?
```javascript
function add(a, b){
	if (a==b) {
  return true
  } else {
  return false
  };
}
```
Is he gonna survive?
```javascript
function hero(bullets, dragons){
if (bullets/2>=dragons) {
return true
} else {
return false
};
}
```
Keep the hoop
```javascript
function hoopCount (n) {
   if (n>=10) {
   return "Great, now move on to tricks"
   } else {
   return "Keep at it until you get it"
   }
}
```
Even or Odd
```javascript
function even_or_odd(number) {
 if (number%2) {
 return "Odd";
 } else {
 return "Even";
 };
 }
```
What's the real floor?
```javascript
function getRealFloor(n) {
if (n==0) {
return 0
} else if (n<0) {
return n
} else if (n==15) {
return n-2
} else if (n>13 && n!=15) {
return n-2
} else {
return n-1
} 
}
```
Calculate BMI
```javascript
function bmi(weight, height) {
let t=weight/(Math.pow(height,2));
if (t<=18.5) {
return "Underweight";
} else if (t<=25.0) {
return "Normal";
} else if (t<=30.0) {
return "Overweight";
} else {
  return "Obese";
  }
}
```
Determine offspring sex based on genes XX and XY chromosomes
```javascript
function chromosomeCheck(sperm) {
  if (sperm.includes('XX')==true) {
  return "Congratulations! You're going to have a daughter."
   } else if (sperm.includes('YX')==true || sperm.includes('XY')==true || sperm.includes('YY')==true) {
  return "Congratulations! You're going to have a son."
  }
}
```
Alan Partridge II - Apple Turnover
```javascript
function apple(x){
if (Math.pow(+x,2)>1000) {
return  'It\'s hotter than the sun!!'
} else {
return 'Help yourself to a honeycomb Yorkie for the glovebox.'
};
}
```

Simple multiplication
```javascript
function simpleMultiplication(number) {
   if (number%2) {
   return number*9
   } else {
   return number*8
   }
}
```

Calculate Two People's Individual Ages
```javascript
function getAges(sum,difference){
let x=difference+(sum-difference)/2;
let y=(sum-difference)/2;
if (sum<0 || difference<0 || x<0 || y<0) {
return null
} else if (x<0 || y<0) {
return null
}else {
return [difference+(sum-difference)/2, (sum-difference)/2]
}
}
```

Sleigh Authentication
```javascript
function Sleigh() {}

Sleigh.prototype.authenticate = function(name, password) {
  if (name=="Santa Claus" && password=="Ho Ho Ho!") {
  return true
  } else {
  return false
  }
}
```

Is n divisible by x and y?
```javascript
function isDivisible(n, x, y) {
if (n%x===0 && n%y===0){
return true
} else {
return false
}
}
```

Is this a triangle?
```javascript
function isTriangle(a,b,c){
   if (a>0 && b>0 && c>0 && a<(b+c) && a>Math.abs(b-c)) {
   return true
   } else {
   return false
   }
}
```
Rock Paper Scissors!

```javascript
const rps = (p1, p2) => {
if (p1=='scissors' && p2=='paper') {
return 'Player 1 won!'
} else if (p1=='paper' && p2=='scissors' ) {
return 'Player 2 won!'
} else if (p1=='scissors' && p2=='rock') {
return 'Player 2 won!'
} else if (p1=='rock' && p2=='scissors'){
return 'Player 1 won!'
} else if (p1=='rock' && p2=='paper') {
return 'Player 2 won!'
} else if (p1=='paper' && p2=='rock'){
return 'Player 1 won!'
} else if (p1=='paper' && p2=='paper' || p1=='scissors' && p2=='scissors' || p1=='rock' && p2=='rock'){
return 'Draw!'
}
}
```

L1: Set Alarm
```javascript
function setAlarm(employed, vacation){
if (employed && vacation){
return false
} else if (!employed && vacation) {
return false
} else if  (employed && !vacation) {
return true
} else if (!employed && !vacation) {
return false
}
}
```

Student's Final Grade

```javascript
function finalGrade (exam, projects) {
 if (exam>90 || projects>10) {
 return 100
 } else if (exam>75 &&projects>=5){
 return 90
 } else if (exam>50 && projects>=2){
 return 75
 } else {
 return 0
 }
}
```







