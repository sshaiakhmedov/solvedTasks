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
Be Concise I - The Ternary Operator
```javascript
// TODO: Refactor and shorten the function
function describeAge(a){
let d="You're a(n) ";
return m=a<13?d+'kid':
(a>12&&a<18)?d+'teenager':
(a>17 &&a<65)?d+'adult':d+'elderly';
}
```
101 Dalmatians - squash the bugs, not the dogs!
```javascript
function howManyDalmatians(number){
  let dogs=["Hardly any", "More than a handful!", "Woah that's a lot of dogs!", "101 DALMATIANS!!!"];
  let respond = number <= 10 ? dogs[0] :
  (number <= 50) ? dogs[1] :
  (number == 101) ? dogs[3] : dogs[2]
return respond;
}
```

Do I get a bonus?
```javascript
function bonusTime(salary, bonus) {
let newSalary;
newSalary=!!bonus ? salary*10 : salary
return "\u00A3"+newSalary
}
```

Training JS #7: if..else and ternary operator
```javascript
function saleHotdogs(n){

  return n<5?100*n:
  (n>=5 && n<10)?95*n:90*n
}
```

Basic Mathematical Operations
```javascript
function basicOp(operation, value1, value2)
{
 switch (operation){
 case '+': return value1+value2;
 break;
 case "-": return value1-value2;
 break;
 case "*": return value1*value2;
 break;
 case "/": return value1/value2;
 break;
 };
}
```





Be Concise I - The Ternary Operator
```javascript
// TODO: Refactor and shorten the function
function describeAge(a){
let d="You're a(n) ";
return m=a<13?d+'kid':
(a>12&&a<18)?d+'teenager':
(a>17 &&a<65)?d+'adult':d+'elderly';
}
```

101 Dalmatians - squash the bugs, not the dogs!
```javascript
function howManyDalmatians(number) {
  
  let dogs = ["Hardly any", "More than a handful!", "Woah that's a lot of dogs!", "101 DALMATIANS!!!"];
  
  let respond = number <= 10 ? dogs[0] : number <= 50 ? dogs[1] : number == 101 ?  dogs[3] : dogs[2]
  
  return respond
  
  }
```
Do I get a bonus?

```javascript

function bonusTime(salary, bonus) {
let newSalary;
newSalary=!!bonus ? salary*10 : salary
return "\u00A3"+newSalary
}
```

Switch it Up!
```javascript
function switchItUp(number){

switch (number){
case 0: return "Zero";
break;
case 1: return "One";
break;
case 2: return "Two";
break;
case 3: return "Three";
break;
case 4: return "Four";
break;
case 5: return "Five";
break;
case 6: return "Six";
break;
case 7: return "Seven";
break;
case 8: return "Eight";
break;
case 9: return "Nine";
break;
}
}
```

simple calculator
```javascript
function calculator(a,b,sign){

switch (sign){
case '+': return a+b;
break;
case '-': return a-b;
break;
case '*': return a*b;
break;
case '/': return a/b;
break;
default: return "unknown value";
}
}
```
power of two
```javascript
function isPowerOfTwo(n){
if (n===1) return true;
while (n>1){
n=n/2
}
if (n===1) {
return true
} else { 
return false;
}
}
```

Difference Of Squares
```javascript
function differenceOfSquares(n){
let sum1=0;
let sum2=0;
  while (n>=1 && n<=100) {
  for (let i=1; i<=n; i++){
  sum1=sum1+i;
  sum2=sum2+Math.pow(i,2);
  }
  return Math.pow(sum1,2)-sum2;
  }
}
```

No zeros for heros
```javascript
function noBoringZeros(n) {
 if (n==0) {
 return 0;
}
while (n%10==0){
n/=10;
}
return n;
}
```

Factorial
```javascript
function factorial(n){
 let f=1;
  for (let i=n; i>=1; i--){
 
  f=f*i;
}
return f;
}
```

Power of 3
```javascript
function largestPower(n){
let k=0;
while (Math.pow(3,k)<n){
k++;
}
   return k-1
}
```

The wheat/rice and chessboard problem
```javascript
function squaresNeeded(grains){
  let square=0;
  let x=1;
  let s=0;
  while (grains>s){
  s+=x;
  x*=2;
  ++square;
  }
  return square;
  }
```

Sum of the first nth term of Series
```javascript
function SeriesSum(n){
if (n==1 || n==0){
return n.toFixed(2);
}
let t=4;
let c=1;
for (let i=1; i<n;i++){
c+=1/t;
t+=3;
}
return c.toFixed(2);
}
```

Grasshopper - Summation
```javascript
let summation = function (num) {
let summ=0;
 for (let i=1; i<=num; i++){
summ+=i;
 }
 return summ;
 }
```

Sum of Multiples
```javascript
function sumMul(n,m){

if (n==0 && m==0) {
return 'INVALID'
} else if (m<0 || n<0){
return 'INVALID'
}
let summ=0;
for (let i=n; i<m; i+=n){
summ+=i;
}
return summ;
}
```

Beginner Series #3 Sum of Numbers
```javascript
function getSum( a,b ){

return ((Math.abs(a-b)+1)*(a+b))/2;
}
```

Draw stairs
```javascript
function drawStairs(n) {
let str="";
  for (let i=1; i<=n; i++){
  str+=i===n? "I" : "I\n" + ' '.repeat(i)
  }
return str;
}
```

Power
```javascript
function numberToPower(number, power) {
let pow=1;
if (power==0){
return pow;
}

let count=1;
    do{
   pow=pow*number;
   count++;
    } while (count<=power);
    return pow;
}
```

Filter the number
```javascript
var FilterString = function(value) {
  let str='';
  for (let i=0; i<value.length; i++){
  if (isNaN(value[i])===false) {
  str+=value[i];
  }
}
return +str;
}
```

isReallyNaN
```javascript
const isReallyNaN = (val) => {
return val!=val
}

```
Is integer safe to use? (1st solution)
```javascript
function SafeInteger(n) {
if (n<=9007199254740991 && n>=-9007199254740991) {
return true
} else {
return false
}
}
```

Is integer safe to use? (2nd solution)
```javascript
function SafeInteger(n) {
return Number.isSafeInteger(n)
}
```
Return Negative
```javascript
function makeNegative(num) {
return  num>0 ? -num : 
 num==0? 0: num;
 
}
```

Opposite number
```javascript
function opposite(number) {
let prod=1;
  return produ=number>=0? number*-prod : -number;
}

```

Invert values
```javascript
function invert(array) {  
for (let i = 0; i < array.length; i++) {
    array[i]=(-1)*array[i];
    }
    return array;
    }
```

BASIC: Making Six Toast.
```javascript
function sixToast(num) {
  return Math.abs(num-6)
}
```

Closest elevator
```javascript
function elevator(left, right, call){
  return Math.abs(call-left)<Math.abs(call-right)? "left":"right";
 }
```

Square Every Digit
```javascript
function squareDigits(num){
let k='';
let c=num.toString();
 for (let i=0; i<c.length; i++){
k+=Math.pow(c[i],2);
 }
 return +k
}
```

Squares sequence
```javascript
function squares(x, n) {

let arr=new Array();
if (n<=0) {
return arr
}
arr[0]=x;
for (let i=1;i<n; i++){

arr[i]=Math.pow(arr[i-1],2);
}
return arr;
}
```

To square(root) or not to square(root)
```javascript
function squareOrSquareRoot(array) {
 for (let i=0; i<array.length; i++){
array[i]=Number.isInteger(Math.sqrt(array[i]))? Math.sqrt(array[i]) : Math.pow(array[i],2);
}
return array
}
```

You're a square!
```javascript
var isSquare = function(n){
 return Number.isInteger(Math.sqrt(n))? true : false
}
```

Find the next perfect square!
```javascript
function findNextSquare(sq) {
return Number.isInteger(Math.sqrt(sq))? Math.pow((Math.sqrt(sq)+1),2) : -1
}
```

Beginner Series #4 Cockroach
```javascript
function cockroachSpeed(s) {
  return Math.floor(s*27.778);
}
```
Price of Mangoes
```javascript
function mango(quantity, price){
return (quantity-Math.floor(quantity/3))*price;
}
```

Holiday VIII - Duty Free
```javascript
function dutyFree(normPrice, discount, hol){
return Math.floor(hol/(normPrice*(discount/100)));
}
```
How many times should I go?
```javascript
function howManyTimes(annualPrice, individualPrice) {
return Math.ceil(annualPrice/individualPrice)
}
```

Tortoise racing
```javascript
function race(v1, v2, g) {
   if (v1>=v2) return null;
   let t=g/(v2-v1);
   let time=t*3600;
   let hour=Math.trunc(time/3600);
   let min=Math.trunc((time-hour*3600)/60);
   let sec=Math.trunc(time-hour*3600-min*60);
   return [hour, min, sec];
}
```
Formatting decimal places #1
```javascript
function twoDecimalPlaces(number) {
return (Math.trunc(number*100))/100
}
```
Lario and Muigi Pipe Problem
```javascript
function pipeFix(numbers){
let arr=new Array();
for (let i=Math.min(...numbers); i<=Math.max(...numbers); i++){
arr.push(i)
}
return arr
}
```
Expressions Matter
```javascript
function expressionMatter(a, b, c) {
let d=a+b*c, e=a*b+c, f=(a+b)*c, h=a*(b+c), k=a+b+c, t=a*b*c;
let arr=[d,e,f,h,k,t];
 return Math.max(...arr)
}
```

Convert to Binary
```javascript
function toBinary(n){
  return Number(n.toString(2));
}
```

Binary Addition
```javascript
function addBinary(a,b) {
return (a+b).toString(2);
}
```
Binary Addition (2nd solution)
```javascript
let addBinary=(a,b)=>(a+b).toString(2);
```

Calculate Price Excluding VAT
```javascript
//return price without vat
function excludingVatPrice(price){
 if (price===null){
  return -1
  } else if (price!==null){
return Number((price/1.15).toFixed(2))
 
  }
}
```

Parse nice int from char problem
```javascript
function getAge (inputString){
for (let i=1; i<=9; i++){
return parseInt(inputString)
}
}
```

Parse nice int from char problem
```javascript
function getAge(inputString){
return parseInt(inputString);
}
```

Hex to Decimal
```javascript
function hexToDec(hexString){
return Number.parseInt(hexString,16);
}
```

Bin to Decimal
```javascript
function binToDec(bin){
return parseInt(bin,2) 
}
```

Parse float
```javascript
function parseF(s) {
  if(Number.isNaN(parseFloat(s)))
    return null;
  else
    return parseFloat(s); 
}
```

Parse float (2nd solution with ternary operator)
```javascript
function parseF(s) {
 return isNaN(parseFloat(s))? null : parseFloat(s);
}
```

Sum Arrays
```javascript
function sum (numbers) {
let summ=0;
if (numbers.length==0) {
return 0
};
for (let i=0; i<numbers.length; i++){
summ+=numbers[i];
}
   return summ; 
}
```
Count the Monkeys!
```javascript
function monkeyCount(n) {
let arr=[];
for (let i=0;i<n;i++){
arr[i]=i+1;
}
return arr;
}
```

Filling an array (part 1)
```javascript
function arr (N){
let arr2=[];
for (let i=0;i<N;i++){
arr2[i]=i;
}
return arr2
}
```
Filling an array (part 1) / 2nd solution with array.push() method
```javascript
function arr (N){
let arr=[];
for (let k=0;k<N;k++){
arr.push(k);
}
return arr;
}
```
What is type of variable?
```javascript
function type(value) {
return ({}.toString.call(value)).slice(8,-1).toLowerCase();

}
```

Is every value in the array an array?
```javascript
function arrCheck (value){
if (value.length==0) return true; 
let count=0;
for (let i=0; i<value.length; i++){
Array.isArray(value[i])==true? count=count+1 : count=count
}
if (count==value.length){
return true
} else {
return false
}
}
```

Enumerable Magic #3 - Does My List Include This?
```javascript
function include(arr, item){
let k=0;
  for (let i=0;i<arr.length; i++){
 if (arr[i]===item){
 k=1;
 break;
}
}
return k==1? true: false;
}
```
Enumerable Magic #3 - Does My List Include This? // solution 2
```javascript
function include(arr, item){
  return arr.includes(item);
}
```

Counting sheep...
```javascript
function countSheeps(arrayOfSheep) {
let count=0;
for (let i=0; i<arrayOfSheep.length; i++){
 if (arrayOfSheep[i]==true){
 count++
}
}
return count;
}
```

A Needle in the Haystack
```javascript
function findNeedle(haystack) {
  // your code here
  let index;
  for (let i = 0; i < haystack.length; i++) {
    if(haystack[i] == 'needle') {
      index = i;
      break;
    }
  }
  return 'found the needle at position ' + index
}
```
A Needle in the Haystack // 2nd solution
```javascript
function findNeedle(haystack) {
return "found the needle at position "+haystack.indexOf("needle");
}
```

Difference of Volumes of Cuboids
```javascript
function findDifference(a, b) {
  return Math.abs(a[0]*a[1]*a[2]-b[0]*b[1]*b[2]);
}
```

Total amount of points
```javascript
function points(games) {
let score=0;
let x;
let y;

for (let i=0;i<games.length; i++){
x=games[i].slice(0,-2);
y=games[i].slice(2);
x>y? score+=3:
x<y? score=score-0:score=score+1;
}
return score;
}
```

Find the first non-consecutive number
```javascript
function firstNonConsecutive (arr) {
let k=0;
let index;
for (let i=0;i<arr.length; i++){
if (arr[i+1]-arr[i]>1) {
index=arr[i+1]
} else if (arr[i+1]-arr[i]==1) {
k++
}
}
return k==arr.length-1? null: index;
}
```

1. Square(n) Sum
```javascript
function squareSum(numbers){
let sum=0;
  for (let i=0;i<numbers.length; i++){
    sum+=Math.pow(numbers[i],2);
}
return sum;
}
```

2. How good are you really?
```javascript
function betterThanAverage(classPoints, yourPoints) {
classPoints.push(yourPoints);
let aver=0;
  for (let i=0; i<classPoints.length; i++){
    aver+=classPoints[i];
  }
return aver/classPoints.length<yourPoints? true : false
}
```

3. Sum of positive

```javascript
function positiveSum(arr) {
let sum=0;
    for (let i=0;i<arr.length; i++){
    if (arr[i]>0) {
    sum+=arr[i];
    }
  }
return sum;
}
```

4. Calculate average
```javascript
function find_average(array) {
  // sum array divided by array length
  let sum = 0;
  for(let i = 0; i < array.length; i++){
    sum += array[i];
  }
  return sum/array.length;
}
```

5. Divide and Conquer
```javascript
function divCon(x){
let strInt=0;
let int=0;
  for (let i=0; i<x.length; i++){
  typeof x[i]=='string'? strInt+=+x[i] : int+=x[i];
  }
  return int-strInt;
}
```

6. Sum of Odd Cubed Numbers
```javascript
function cubeOdd(arr) {
let oddCubed=0;
  for (let i=0; i<arr.length; i++){
  if (!Number.isInteger(arr[i])){
  return undefined
  }
  Math.abs(arr[i]%2)===1? oddCubed+=Math.pow(arr[i],3) : oddCubed=oddCubed;
  }
return oddCubed;
}
```

7. Odd or Even?
```javascript
function oddOrEven(array) {
let sum=0;
  for (let i=0; i<array.length; i++){
  sum+=array[i];
  }
  return sum%2==0? 'even' : 'odd';
}
```

8. Find the smallest integer in the array
```javascript
class SmallestIntegerFinder {
  findSmallestInt(args) {
    return Math.min(...args);
  }
}
```

9. Remove the minimum
```javascript
function removeSmallest(numbers) {
let k=numbers.indexOf(Math.min(...numbers));
let arr=new Array();
  for (let i=0; i<numbers.length; i++){
  if (i!=k) {
    arr.push(numbers[i]);
    }
  }
return arr;
}
```

* 28-Dec
1. Sum without highest and lowest number
```javascript
function sumArray (array) {
  if (array==undefined || array==null){
  return 0;
  } else if (!array[2]){
  return 0;
  }
    let min=array.indexOf(Math.min(...array));
    let max=array.indexOf(Math.max(...array));
    let sum=0;
    for (let i=0; i<array.length; i++){
    sum+=array[i]
    }
  
return sum-array[min]-array[max];
}
```

2. Find Maximum and Minimum Values of a List
```javascript
let min = function (list){
    
    return Math.min(...list);
}

let max = function (list){
    
    return Math.max(...list);
}
```

3. Reversed sequence
```javascript
const reverseSeq = n => {
let arr=new Array ();
  for (let i=n; i>=1; i--){
  arr.push(i)
  }
return arr;
}
```

4. Unfinished Loop - Bug Fixing #1
```javascript
function createArray(number){
  var newArray = [];
  
  for (let counter = 1; counter <= number; counter++){
    newArray.push(counter);
  }
  
  return newArray;
}
```

5. Training JS #10: loop statement --for
```javascript
function pickIt(arr){
  var odd=[],even=[];
  
  for (let i=0;i<arr.length; i++){
    if (arr[i]%2==0){
    even.push(arr[i])
    } else {
    odd.push(arr[i]);
    }
  }
  
  return [odd,even];
}
```

6. Pre-FizzBuzz Workout #1
```javascript
function preFizz(n) {
//n>=1
let arr=[]; //or let arr=new Array();
let i=1;
  while (i<=n){
  arr.push(i);
  i++
  }
  return arr;
}
```

7. Count by X
```javascript
function countBy(x, n) {
let arr=[];
  for (let i=1; i<=n; i++){
  arr.push(i*x);
  }
return arr;
}
```

8. Powers of 2
```javascript
function powersOfTwo(n){
//n>0
/*Math.pow(n,0...n)*/
let arr=new Array();
  for (let i=0;i<=n; i++){
  arr.push(Math.pow(2,i));
  }
return arr;
}
```

9. Find the divisors!
```javascript
function divisors(integer) {
//exclude 1 and integer in array

  if (integer%2!=0 && integer%3!=0 && integer%5!=0 && integer%11!=0 || integer==3 ) {
  return `${integer} is prime`;
  }
  
  let arr=[]; //2nd: let arr=new Array();
  for (let i=2; i<integer; i++){
    if (integer%i==0 && i<=integer){
    arr.push(i);
   }
  }
return arr;
}
```

10. Training JS #4: Basic data types--Array
```javascript
function getLength(arr){
  return arr.length;
}

function getFirst(arr){
  return arr[0];
}

function getLast(arr){
  //return the last element of arr
  return arr[arr.length-1];
}

function pushElement(arr){
  var el=1;
  arr.push(el);
  //push el to arr
  return arr
}

function popElement(arr){
  //pop an element from arr
 arr.pop(); 
```

11. o Loops 2 - You only need one
```javascript
function check(a,x){
return a.includes(x)? true : false;
}
```
11. o Loops 2 - You only need one // 2nd solution
```javascript
let check =(a,x)=> a.includes(x);
```

12. You only need one - Beginner
```javascript
let check=(a, x)=> a.includes(x);
```

13. Be Concise IV - Index of an element in an array
```javascript
let find=(array,element)=>{return array.includes(element)?array.indexOf(element):"Not found"}
```

14. A wolf in sheep's clothing
```javascript
function warnTheSheep(queue) {
  
  return queue.indexOf("wolf")===queue.length-1? "Pls go away and stop eating my sheep" : `Oi! Sheep number ${queue.length-queue.indexOf("wolf")-1}! You are about to be eaten by a wolf!`
}
```
14. A wolf in sheep's clothing // 2nd method
```javascript
function warnTheSheep(queue) {
let position=queue.reverse().indexOf("wolf");
return position===0? "Pls go away and stop eating my sheep" : `Oi! Sheep number ${position}! You are about to be eaten by a wolf!`
}
```

#29-Dec

1. JavaScript Array Filter
```javascript
let getEvenNumbers =(numbersArray)=>numbersArray.filter(el=>el%2===0);
```

2. Find numbers which are divisible by given number
```javascript
let divisibleBy=(numbers, divisor)=> numbers.filter(el=>el%divisor===0);
```

3. Removing Elements
```javascript
function removeEveryOther(arr){
  return arr.filter((el,ind)=>ind%2===0)
}
```

4. filterEvenLengthWords
```javascript
let filterEvenLengthWords=words=> words.filter(el=> el.length%2===0);
```

5. Find how many times did a team from a given country win the Champions League?
```javascript
let countWins=(winnerList, country)=> (winnerList.filter(el=>el.country==country)).length;
```

6.  Well of Ideas - Easy Version /1st solution
```javascript
function well(x){
if (x.includes('bad') && !x.includes('good') || !x.includes('bad') && !x.includes('good')) return "Fail!";
let k=0;
    for (let i=0; i<x.length; i++){
     
     x[i].includes('good')? k++ : k=k;
      }
    if (k>2) {
    return 'I smell a series!'
    } else {
    return "Publish!"
    }
}
```
6. Well of Ideas - Easy Version  / 2nd soulution with array.filter
```javascript
function well(x){
let countGood=x.filter(el=>el=='good').length;
return countGood<1? 'Fail!':
      countGood<3?  'Publish!': 'I smell a series!';
}
```
7. Array.diff
```javascript
function array_diff(a, b) {
 return a.filter(el=>!b.includes(el));
}
```

8. Find Duplicates
```javascript
function duplicates(arr) {
return arr.filter((el,ind)=> ind==arr.indexOf(el) && ind!=arr.lastIndexOf(el));
}
```

30-Dec-19

1. Train to remove duplicates from an array with filter()
```javascript
let unique=arr=> arr.filter((el,i)=>i==arr.indexOf(el));
```
2. Santa's Naughty List
```javascript
function findChildren(santasList, children) {
return santasList.filter((name, ind)=> children.includes(name) && ind==santasList.indexOf(name)).sort();
}
```

3. Convert number to reversed array of digits
```javascript
function digitize(n) {
let arr= n.toString().split("").reverse();
for (let i=0; i<arr.length; i++){
  arr[i]*=1;
  }
  return arr
}
```

4. My head is at the wrong end!
```javascript
function fixTheMeerkat(arr) {
 return arr.reverse();
}
```

5. Two Oldest Ages
```javascript
function twoOldestAges(ages){
let arr2=ages.sort((a,b)=>a-b);
return arr2.filter((el,ind)=>ind>=arr2.length-2);
}
```

6. Sum of two lowest positive integers
```javascript
function sumTwoSmallestNumbers(numbers) {  
let arr=numbers.sort((a,b)=>a-b);
return arr[0]+arr[1];
}
```

7. Sentence Smash
```javascript
function smash (words) {
return words.join(' ');
};
```

8. String Templates - Bug Fixing #5
```javascript
let buildString=(...array)=>"I like "+ array.join(', ') +"!";
```

9. Printing Array elements with Comma delimiters
```javascript
function printArray(array){
  return array.join();
}
```

10. CSV representation of array
```javascript
function toCsvText(array) {
  return array.join('\n');
}
```

11. Enumerable Magic #1 - True for All?
```javascript
function all( arr, fun ){
  return arr.every(fun) ? true : false;
}
```

12. Grasshopper - Array Mean
```javascript
let findAverage = nums=> nums.reduce((acc,curr)=>acc+curr)/nums.length;
```

13. Beginner - Reduce but Grow
```javascript
function grow(x){
return x.reduce((acc,curr)=>acc*curr,1);
}
```

14. Array plus array
```javascript
function arrayPlusArray(arr1, arr2) {
  return arr1.reduce((acc,el)=>acc+el,0) + arr2.reduce((acc,el)=>acc+el); //something went wrong
}
```

15. SpeedCode #2 - Array Madness
```javascript
function arrayMadness (a, b) {
return a.reduce((acc, curr) => acc + curr**2, 0) > b.reduce((acc, curr) => acc+ curr**3, 0)? true : false;
}
```

16. Beginner - Lost Without a Map
```javascript
function maps(x){
return x.map(el=>el*2);
}
```

17. Enumerable Magic #25 - Take the First N Elements
```javascript
function take(arr, n) {
  return arr.splice(0,n);
}
```























