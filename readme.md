#### 7) Create a README file to answer the following question-


#### 1) What is the difference between var, let, and const?
Answer:-) var, let, and const

var → Old way to create a variable. Can be changed and re-declared anywhere in the function.

let → New way. Can be changed but cannot re-declare in the same block.

const → New way. Cannot be changed (but if it’s an object/array, the contents can change).

Example:

var x = 10;
x = 20;          // OK
var x = 30;      // OK

let y = 5;
y = 6;           // OK
// let y = 7;    // ❌ Error: cannot re-declare

const z = 100;
// z = 200;      // ❌ Error: cannot change
const arr = [1,2];
arr.push(3);     // ✅ OK: array content can change

#### 2) What is the difference between map(), forEach(), and filter()? 
Answer:-forEach, map, filter

forEach → Go through each item, do something, returns nothing.

map → Go through each item, make a new array with changes.

filter → Go through each item, make a new array with only the items that match a condition.

Example:

const numbers = [1,2,3];

numbers.forEach(n => console.log(n));     // prints 1, 2, 3

const doubled = numbers.map(n => n*2);   // [2, 4, 6]
const even = numbers.filter(n => n%2===0); // [2]

#### 3) What are arrow functions in ES6?
Answer:-Arrow Functions

Short way to write functions:

const add = (a, b) => a + b;
console.log(add(2,3)); // 5

Arrow functions use this from outside, cannot be used as new functions.

#### 4) How does destructuring assignment work in ES6?
Answer:-Destructuring

Easy way to take values from arrays or objects:

Array example:

const arr = [10, 20];
const [a, b] = arr;  // a=10, b=20

Object example:

const person = {name:'Ali', age:30};
const {name, age} = person;
console.log(name, age); // Ali 30

#### 5) Explain template literals in ES6. How are they different from string concatenation?
Answer:-Template Literals

Use backticks ` instead of quotes.

Can put variables inside using ${} and write multi-line text easily.

const name = "Asha";
const msg = `Hello, ${name}!
How are you today?`;
console.log(msg);

Normal way with + is harder:

const msg2 = "Hello, " + name + "!\nHow are you today?";
