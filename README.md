## Codewar Katas
##### Solved katas from https://codewars.com

* My wi-fi doesn't allow me to download the Git for 3-4 time. I will update repository from gitHub.
* JS Practise: Section 2.2 (solved around 8 CW tasks).
* 11-Dec-2019. JS Practise. Reached 2-3 + LEcture with Vladimir.
* 12-Dec-2019. Java Class with Sergey. JSP. Installed and set up Git

1. Convert a String to a Number!
```javascript
let stringToNumber = function(str){
  return Number(str);
}
```
2. Sum The Strings
```javascript
function sumStr(a,b) {
  a=+a;
  b=+b;
  return String(a+b);
}
```
3. Century From Year 
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
4. Count Odd numbers below n
```javascript
function oddCount(n) {
     return Math.floor(n/2);
}
```
5. Return the closest number multiple of 10
```javascript
const closestMultiple10 = num => {
if (num<10) {
return 10
} else {
return Math.round(num/10)*10;
}
}
```
6. Area of a Square
```javascript
function squareArea(A){
  return +Math.pow((4*A)/(2*Math.PI),2).toFixed(2);
}
```
7. Formatting decimal places #0
```javascript
function twoDecimalPlaces(n) {
  return +n.toFixed(2);
}
```
8. Discover The Original Price
```javascript
function discoverOriginalPrice(discountedPrice, salePercentage){
  return +((discountedPrice*100)/(100-salePercentage)).toFixed(2);
}
```
9. Simple Comparison?
```javascript
function add(a, b){
	if (a==b) {
  return true
  } else {
  return false
  };
}
```
10. Is he gonna survive?
```javascript
function hero(bullets, dragons){
if (bullets/2>=dragons) {
return true
} else {
return false
};
}
```
11. Keep the hoop
```javascript
function hoopCount (n) {
   if (n>=10) {
   return "Great, now move on to tricks"
   } else {
   return "Keep at it until you get it"
   }
}
```
12. Even or Odd
```javascript
function even_or_odd(number) {
 if (number%2) {
 return "Odd";
 } else {
 return "Even";
 };
 }
```
13. What's the real floor?
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
14. Calculate BMI
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
15. Determine offspring sex based on genes XX and XY chromosomes
```javascript
function chromosomeCheck(sperm) {
  if (sperm.includes('XX')==true) {
  return "Congratulations! You're going to have a daughter."
   } else if (sperm.includes('YX')==true || sperm.includes('XY')==true || sperm.includes('YY')==true) {
  return "Congratulations! You're going to have a son."
  }
}
```
16. Alan Partridge II - Apple Turnover
```javascript
function apple(x){
if (Math.pow(+x,2)>1000) {
return  'It\'s hotter than the sun!!'
} else {
return 'Help yourself to a honeycomb Yorkie for the glovebox.'
};
}
```

17. Simple multiplication
```javascript
function simpleMultiplication(number) {
   if (number%2) {
   return number*9
   } else {
   return number*8
   }
}
```

18. Calculate Two People's Individual Ages
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

19. Sleigh Authentication
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
20. Is n divisible by x and y?
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

31-dec

1. Remove First and Last Character Part Two / in progress
```javascript
function array(str){
let str1=str.split(',').slice(1,-1).join(' ');
return str1.length>0? str1 : null;
}
``` 

# 01-JAn-2020

1. Jenny's secret message
```javascript
function greet(name){
  
  if (name === "Johnny"){
    return "Hello, my love!";
    } else {
   return  "Hello, " + name + "!"
    }
}
```

2. Template Strings
```javascript
var TempleStrings = function(obj, feature) {
  return obj+" are "+feature;
}
```

3. Returning Strings
```javascript
function greet(name){
return `Hello, ${name} how are you doing today?`
}
```

4. Grasshopper - Combine strings
```javascript
function combineNames(a,b){
return `${a} ${b}`;
}
```

5. If you can't sleep, just count sheep!!
```javascript
var countSheep = function (num){
let str='';
  for (let i=1;i<=num;i++){
  str+=`${i} sheep...`;
  }
  return str;
}
```

6. Grasshopper - Debug sayHello
```javascript
function sayHello (name) {
return "Hello, "+name;
}
```

7. get character from ASCII Value
```javascript
function getChar(c){
return String.fromCodePoint(c);
}
```

8. Regex validate PIN code
```javascript
function validatePIN (pin) {
 return Number.isInteger(+pin) && !pin.includes('e') && pin.length===4 && !pin.includes('\n') && !pin.includes('+') && !pin.includes('-') && !pin.includes(' ') && !pin.includes('.')  || +pin==0000 && pin.length==4 || +pin==000000 && pin.length==6 || Number.isInteger(+pin) && pin.length===6 && !pin.includes('-') && !pin.includes(' ','') && !pin.includes('+') && !pin.includes('.') && !pin.includes(' ') && !pin.includes('\n')  ? true : false;
 }

```

9. Is this my tail?
```javascript
function correctTail (body, tail) {
return body.charAt(body.length-1)==tail
}
```

#02-Jan-2019

1. 5 without numbers !!
```javascript
function unusualFive() {
return ['s','s','s','s','s'].length
}
```
2. Numbers to Letters
```javascript
function switcher(x){
  const alp = "0zyxwvutsrqponmlkjihgfedcba!? ";
  return x.map((el, i) => el = alp[el]).join('');
}
```
Solution 2:
```javascript
function switcher(x){
  let letters = "0zyxwvutsrqponmlkjihgfedcba!? ";
  const arr = [];
  for (let i = 0; i < x.length; i++) {
    arr.push(letters[x[i]]);
  }
  return arr.join('');
}
```
3. Abbreviate a Two Word Name
```javascript
function abbrevName (name){

let arr=name.split(' ');

let initials=`${arr[0].charAt(0)}.${arr[1].charAt(0)}`;
return initials.toUpperCase();
}
```

# 03-Jan

1. Regex count lowercase letters
```javascript
function lowercaseCount(str){
let count=0;
   for (let i=0;i<str.length; i++){
   if (str[i]!=str[i].toUpperCase()){
   count+=1;
   }
  }
   return count
}
```

2. Double Char
```javascript
function doubleChar(str) {
 let arr=str.split('');

 return arr.map(el=>el+el).join('');
}
```

3. Remove First and Last Character
```javascript
function removeChar(str){
 
let arr=str.split('');
arr.pop();
arr.shift();
return arr.join('');
};

```

4. Triple Trouble
```javascript
function tripleTrouble(one, two, three){
let arr=[];
  for (let i=0;i<one.length; i++){
  arr.push(one[i]);
  arr.push(two[i]);
  arr.push(three[i]);
  }
  return arr.join('');
 }
```

5. Remove String Spaces
```javascript
function noSpace(x){
let arr= x.split('');
let arr2=[];

for (let i=0; i<arr.length; i++) {
 arr[i]!=" "?  arr2.push(arr[i]) : arr2=arr2;
  }
return arr2.join('');
}
```

6. Spacify
```javascript
function spacify(str) {
 return str.split('').join(' ');
}
```

7. Unique In Order
```javascript
var uniqueInOrder=function(iterable){
let arr2=[];
  if (Array.isArray(iterable)){
   for (let i=0;i<iterable.length; i++){
  if (iterable[i+1]!=iterable[i]){
    arr2.push(iterable[i])
      }
    }
  return arr2;
  } else {
let arr1=iterable.split('');

for (let i=0;i<arr1.length; i++){
  if (arr1[i+1]!=arr1[i]){
    arr2.push(arr1[i])
    }
  }
}
return arr2;
}
```

7. Unique In Order / 2nd solution
```javascript
var uniqueInOrder=function(iterable){
 let arr=[];
 for (let i=0; i<iterable.length; i++){
 if (iterable[i+1]!=iterable[i]){
 arr.push(iterable[i])
}
}
return arr
}
```

8. Reversed Strings
```javascript
function solution(str){
  let arr=str.split('');
  return arr.reverse().join('');
}
```

9. Is it a palindrome?
```javascript
function isPalindrome(x) {
  return x.toUpperCase()==x.toUpperCase().split('').reverse().join('')
}
```

10. The Wide-Mouthed frog!
```javascript
function mouthSize(animal) {
 return animal.toLowerCase()=='alligator'? 'small' : "wide"
}
```

11. Find the capitals
```javascript
var capitals = function (word) {
	let arr=[];
  for (let i=0;i<word.length; i++){
    if (word[i]==word[i].toUpperCase()){
    arr.push(i)
    }
  }
return arr;
};
```

12. Capitalization and Mutability
```javascript
function capitalizeWord(word) {
let arr=word.split('');
arr[0]=arr[0].toUpperCase();
return arr.join('');
}
```

13. MakeUpperCase
```javascript
function makeUpperCase(str) {
  return str.toUpperCase();
}
```

14. Thinking & Testing : Something capitalized
```javascript
function testit(s){
let arr=s.split('');

  for (let i=0; i<arr.length; i++){
    if (arr[i+1]==' ' || arr[i+1]==undefined){
    arr[i]=arr[i].toUpperCase();
    }
  }
return arr.join('');
}
```

15. Mumbling
```javascript
function accum(s) {
s.split('');
const arr=[];
  for (let i=0;i<s.length; i++){
  let x=s[i].toUpperCase();
    for (let k=0; k<i; k++){
    x+=s[i].toLowerCase();
    }
    arr.push(x);
  }
  return arr.join('-'); 
}
```

#01-04-2020

1. repeatIt
```javascript
var repeatIt = function(str, n) {
return typeof str=='string'? str.repeat(n) : 'Not a string';
  }
```

2. String repeat
```javascript
function repeatStr (n, s) {
  return s.repeat(n);
}
```

3. Do you speak "English"?
```javascript
function spEng(sentence){
let c='English'
return sentence.toUpperCase().includes(c.toUpperCase());
}
```

4. Don't give me five!
```javascript
function dontGiveMeFive(start, end) {
let count=0;
  for (let i=start; i<=end; i++){
  !String(i).includes(5)? count++ : count
  }
return count
}
```

5. Find the position!
```javascript
function position(letter){
let alph=' abcdefghijklmnopqrstuvwxyz';
return `Position of alphabet: ${alph.indexOf(letter)}`;
}
```

6. validate code with simple regex
```javascript
function validateCode (code) {
  if (String(code).startsWith(1) || String(code).startsWith(2) || String(code).startsWith(3)){
    return true
    } else {
   return false
  }
}
```

7. String ends with?
```javascript
function solution(str, ending){
  return str.endsWith(ending);
}
```
#05-Jan-2020

1. Credit Card Mask
```javascript
// return masked string
function maskify(cc) {
if (cc.length<=4){
return cc
}
let a=cc.slice(cc.length-4);
let b=cc.slice(0,-4);
let c='';
  for (let i=1;i<=b.length;i++){
  c+='#'
  }
  return c+a;
}
```

2. Tail Swap
```javascript
function tailSwap(arr) {
let a1=arr[0].lastIndexOf(':');
let b2=arr[1].lastIndexOf(':');
let a=arr[0].slice(a1);
let b=arr[1].slice(b2);

let arr2=[];
arr2[0]=arr[0].slice(0,a1)+b;
arr2[1]=arr[1].slice(0,b2)+a;
  return arr2;
}
```

3. Vowel remover
```javascript
function shortcut (string) {
let vowel='aeiouy';
return string.replace(/[a,e,i,o,u]/gi,'');
}
```
2nd solution
```javascript
function shortcut(string){
return string.replace(/[aeiou]/ig,'');
}
```

4. DNA to RNA Conversion
```javascript
function DNAtoRNA(dna) {
return dna.replace(/[T]/g, 'U');
}
```
2nd solution without []
```javascript
function DNAtoRNA(dna) {
return dna.replace(/T/g, 'U');
}
```

5. Get number from string
```javascript
function getNumberFromString(s) {
  return +s.replace(/\D/g,'');
}
``` 

6. Fake Binary
```javascript
function fakeBin(x){
return x.replace(/[1,2,3,4]/g,'0').replace(/[5-9]/g,'1');
}
```

7. Correct the mistakes of the character recognition software
```javascript
function correct(string){
return string.replace(/5/g,'S').replace(/0/g,'O').replace(/1/g,'I');
}
```

8. IXME: Replace all dots
```javascript
var replaceDots = function(str) {
  return str.replace(/[.]/g, '-');
}
```

9. Exclamation marks series #2: Remove all exclamation marks from the end of sentence
```javascript
function remove(s){
return s.replace(/!+$/g,'')
}

```

10. Reversed Words
```javascript
function reverseWords(str){
 return str.split(' ').reverse().join(' ')
}
```

11. Descending Order
```javascript
function descendingOrder(n){
  n=String(n);
  let k=n.split('').sort((a,b)=>b-a).join('');
  return k*1
}
```

12. Highest and Lowest
```javascript
function highAndLow(numbers){
  let arr=numbers.split(' ');
  let arr2=arr.sort((a,b)=>b-a);
  return `${arr2[0]} ${arr2[arr2.length-1]}`;
}
```

13. Squash the bugs
```javascript
function findLongest(str) {
  
  let spl = str.split(' ');
  let longest = 0;
  
    for (let i = 0; i<spl.length; i++) {
      if (spl[i].length > longest) {
      longest = spl[i].length
      }
    }
  return longest
}
```

14. Reversing Words in a String
```javascript
function reverse(string){
  let arr=string.split(' ');
  return arr.reverse().join(' ')
}
```

15. Convert a string to an array
```javascript
function stringToArray(string){
return string.split(/\s{1,}/);
}
```

16. Can Santa save Christmas?
```javascript
function determineTime(durations){
let arr=durations.join().replace(/,/g,':').split(':');
let hr=0, min=0, sec=0;
  for (let i=0, j=1, k=2; i<arr.length, j<arr.length, k<arr.length; i+=3, j+=3, k+=3){
  hr+=+arr[i];
  min+=+arr[j];
  sec+=+arr[k];
  } 
  let sum=hr+min/60+sec/60;
return sum<=24? true : false;
}
```

#06-Jan-2020

1. Every possible sum of two digits
```javascript
function digits(num){
let arr=String(num).split('');
let arr2=[];

  for (let i=0, j=1; i<arr.length, j<arr.length; i++, j++){
 
    for (let k=j; k<arr.length; k++){
    arr2.push(+arr[i]+(+arr[k]));
    
    }
    
  }
return arr2
}
```

#07-Jan-2020

1. Welcome!
```javascript
function greet(language) {
let langDb={
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
};
return ([language] in langDb)? langDb[language] :langDb.english;
}
```

2. Duck Duck Goose
```javascript
function duckDuckGoose(players, goose) {
  return players[(goose - 1) % players.length].name;
}
```

3. What is between?
```javascript
function between(a, b) {
let arr=[];
for (let i=a;i<=b; i++){
arr.push(i);// your code here
}
return arr
}
```

4. Sum Mixed Array
```javascript
function sumMix(x){
return x.reduce((acc,cur)=>+acc+Number(cur));
}
```

5. Sort and Star
```javascript
function twoSort(s) {
return s.sort()[0].split('').join('***');
}
```

# 08-Jan-2020

1. makeBackronym
```javascript
//preload variable: dict

let makeBackronym = function(string){
let arr=string.split('');
let arrNew=[];
  for (let i=0;i<arr.length; i++){
  arrNew.push(dict[arr[i].toUpperCase()])
  }
return arrNew.join(' ')
};
```

2. Make a function that does arithmetic!
```javascript
function arithmetic(a, b, operator){
  let obj={
    add: a+b,
    subtract: a-b,
    multiply: a*b,
    divide: a/b, 
  }
 return obj[operator]  
}
```

3. Check three and two
```javascript
function checkThreeAndTwo(array) {
let aC=0, bC=0, cC=0;
  for (let i=0; i<array.length; i++){
  array[i]=="a"? aC++:
  array[i]=="b"? bC++: cC++;
  }
return aC==2 && bC==3 || aC==3 && bC==2 || aC==2 && cC==3 || aC==3 && cC==2 || bC==2 && cC==3 || bC==3 && cC==2? true : false
}
```

4. Job Matching #1
```javascript
function match(candidate, job) {
  if (!!job.maxSalary && !!candidate.minSalary){
    return job.maxSalary + candidate.minSalary * 0.1 >= candidate.minSalary;
  } else {
    throw 'Error';
  }
}
```

5. Multiple of index
```javascript
function multipleOfIndex (array) {
  let arr=[];
  for (let i=0; i<array.length; i++){
    if (array[i]%i==0) {
    arr.push(array[i]);
    }
  }
  return arr;
}
```

#09-Jan-2020

1. Add property to every object in array
```javascript
 
questions.forEach(el => el.usersAnswer = null);
```

#### 10-Jan=2020

1. Numbers to Objects
```javascript
function numObj(s){
let arr=[];

  for (let i=0; i<s.length; i++) {
    arr[i]={};
  arr[i][s[i]]=String.fromCharCode(s[i]);
  }
  return arr;
}
```

2. Coding Meetup #5 - Higher-Order Functions Series - Prepare the count of languages
```javascript
function countLanguages (list){
  const arr = [];
  let obj = {};
  for (i = 0; i < list.length; i++){
    arr.push(list[i]['language'] )
  }
  for (i = 0; i < arr.length; i++){
    if (obj.hasOwnProperty(arr[i]) ) {
      obj[arr[i]]++;
    } else {
      obj[arr[i]] = 1;
    }
  }
  return obj;
}
```

##### 11-Jan-2020

1. Most valuable character
```javascript
function solve(st) {
  const obj = {}, ordered = {};
  for (let el of st){
    if (!obj.hasOwnProperty(el)) obj[el] = st.lastIndexOf(el) - st.indexOf(el);
  }
  let max = Math.max(...Object.values(obj));
  Object.keys(obj).sort().forEach(key => ordered[key] = obj[key]);
  for (let key in ordered){
    if(ordered[key] === max) return key;
  }
}
```

2.  What is my name score? #1
```javascript
function nameScore(name){
let arrName=name.toUpperCase().split(''); //new Array of name

let arr=[];
arr=Object.keys(alpha).join('').split(''); // newa array of alphabet letters

let tr=0;
for (let el in arrName){
  for (let key in alpha){
  if (key.includes(arrName[el])) 
    tr+=alpha[key]
  }
}
let ob={};
ob[name]=tr;
return ob
}
```

3. The Office I - Outed
```javascript
function outed(meet, boss){
// let meet={
//   'tim':0,
//   'jim':2,
//   'randy':0,
//   'sandy':7,
//   'andy':0,
//   'katie':5,
//   'laura':1,
//   'saajid':2,
//   'alex':3,
//   'john':2,
//   'mr':0
// };
//let boss='jim';
let bossScore=0;
for (let key in meet){
  if (key==boss) bossScore=meet[key];
};
//console.log(bossScore);

let arr=[];
arr=Object.keys(meet); //array with attendies to get the number of attendies
//console.log(arr);
let n=arr.length; //number of attendees

let arr2=[];
for (let key in meet){
arr2.push(meet[key])
};

let score=arr2.reduce((acc,cur)=>acc+cur, bossScore)
//console.log(score);
//console.log(arr2);
let meetScore=score/n;

return meetScore<=5?  'Get Out Now!' : 'Nice Work Champ!';
}
```

4. How many days are we represented in a foreign country?
```javascript
function daysRepresented(trips){
  const days = [];
  for (i = 0; i < trips.length; i++) {
    for (j = trips[i][0]; j <= trips[i][1]; j++) {
      if (!days.includes(j)) days.push(j);
    }
  }
  return days.length;
}
```

5.  Permute a Palindrome
```javascript
function permuteAPalindrome(input) {
  let count = 0;
  const dict = input.split``.reduce(
    (a, b) => ((a[b] = a[b] ? a[b] + 1 : 1), a),
    {}
  );
  for (let i in dict) {
    if (dict[i] % 2 !== 0) {
      count++;
    }
    if (count === 2) return false;
  }
  return true;
}
```

##### 12-Jan-2020

1.  Keep Hydrated!
```javascript
function litres(time) {
  if (time%2==0) {
  return drink=time*0.5}
  else {return drink=Math.floor(time*0.5)
}
```

2. ilter out the geese
```javascript
function gooseFilter (birds) {
  let geese = ["African", "Roman Tufted", "Toulouse", "Pilgrim", "Steinbacher"];
return birds.filter(el=>!geese.includes(el))
};
```

3. Will there be enough space?
```javascript
function enough(cap, on, wait) {
  return cap-on>=wait? 0 : wait-cap+on;
}
```

4. Flatten and sort an array
```javascript
"use strict";

function flattenAndSort(array) {
 
let arr2=[];
array.map(el=>el.map(el2=>arr2.push(el2)));
return arr2.sort((a,b)=>a-b);
}
```

5. Is the string uppercase?
```javascript
String.prototype.isUpperCase = function () {
return  this.toUpperCase()===this.toString();
}
```

#### 13-Jan=2020

1. Will you make it?
```javascript
const zeroFuel = (distanceToPump, mpg, fuelLeft) => {
  return fuelLeft*mpg>=distanceToPump? true : false;
};
```

2. You Can't Code Under Pressure #1
```javascript
let doubleInteger=i=>i*2;
```

3. Watermelon
```javascript
function divide (w){
  // 1<=w<=100
  return w%2==0 && w>2
}
```

4.  Grasshopper - Messi goals function
```javascript
function goals (laLigaGoals, copaDelReyGoals, championsLeagueGoals) {
return laLigaGoals+copaDelReyGoals+championsLeagueGoals;
}
```

5. Shortest Word
```javascript
function findShort(s){
let arr=s.split(' ');

let count=arr[0].length;
for (let el in arr){
  if (arr[el].length<count){
    count=arr[el].length
  }
}
return count
}
```

#### 14-Jan-2020

1. Tip Calculator
```javascript
function calculateTip(amount, rating) {
return rating.toLowerCase()=='Terrible'.toLowerCase()? Math.ceil(amount*0) :
rating.toLowerCase()=='Poor'.toLowerCase()? Math.ceil(amount*0.05) :
rating.toLowerCase()=='Good'.toLowerCase()? Math.ceil(amount*0.1) :
rating.toLowerCase()=='Great'.toLowerCase()? Math.ceil(amount*0.15) :
rating.toLowerCase()=='Excellent'.toLowerCase()? Math.ceil(amount*0.2) : "Rating not recognised";
}
```

2. Grasshopper - Personalized Message
```javascript
function greet (name, owner) {
return name==owner? 'Hello boss' : 'Hello guest'
}
```

3. Grasshopper - Terminal game move function
```javascript
function move (position, roll) {
return position+roll*2
}
```

4. Grasshopper - Check for factor
```javascript
function checkForFactor (base, factor) {
return base%factor==0? true : false
}
```

5. Get Nth Even Number
```javascript
function nthEven(n){
return n*2-2
}
```

#### 15-Jan

1. Grasshopper - Terminal game combat function
```javascript
function combat(health, damage) {
return health-damage>0? health-damage : 0
}
```

2. How many lightsabers do you own?
```javascript
function howManyLightsabersDoYouOwn(name) {
  return name=="Zach"? 18 : 0
}
```

3.  Is there a vowel in there?
```javascript
function isVow(a){
let vow=['a','e','i','o','u'];
for (let el2 in vow){
  for (let el in a){
    if (vow[el2]==String.fromCharCode(a[el])){
      a[el]=vow[el2]
      }
    }
}
return a
}
```

4. Get the mean of an array
```javascript
function getAverage(marks){
return Math.floor(marks.reduce((acc,cur)=>acc+cur)/marks.length)
}
```

5. Palindrome Strings
```javascript
function isPalindrome(line) {
  return line==line.split('').reverse().join('')
}
```

#### 16-Jan

1. Return the day
```javascript
 function whatday(num) { 
 let day=num;
switch (num){
  case 1: return "Sunday"
  break;
  case 2: return "Monday"
  break
  case 3: return "Tuesday"
  break;
  case 4: return "Wednesday"
  break;
  case 5: return "Thursday"
  break;
  case 6: return "Friday"
  break;
  case 7: return "Saturday"
  break;
  default: return "Wrong, please enter a number between 1 and 7";
  }
```

2. get ascii value of character
```javascript
function getASCII(c){
  return c.charCodeAt()
}
```

3. All Star Code Challenge #18
```javascript
function strCount(str, letter){  
 return str.split('').filter(el=>el==letter).length
}
```

4. Find Nearest square number
```javascript
function nearestSq(n){
    return Math.round(Math.pow(n,1/2))**2
}
```

5. Remove exclamation marks
```javascript
function removeExclamationMarks(s) {
  return s.split('').filter(el=>el!='!').join('')
}
```