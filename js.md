## What is a Variable?
A variable is like a box where you can store information.

For example:

You want to store your name = "Shivani"<br>
You want to store your age = 15<br>
You use a variable to do that in JavaScript.

 ## How to Declare Variables?
In JavaScript, we use let and const to declare variables.

 1. let – This is for values that can change
javascript<br>
let age = 15;<br>
console.log(age); // Output: 15

age = 16; // we changed the value<br>
console.log(age); // Output: 16


 2. const – This is for values that cannot change
javascript

const name = "Shivani";<br>
console.log(name); // Output: Shivani

if name= ayesha then it will give error

### Important difference

| feature      | `let`       | `const`        |
|--------------|-------------|----------------|
|Can change?   |yes           | no            |
|Re-declare?   |no            | no            |
|Used for?     |the values which changes|for fixed values|

## What are Data Types?
In JavaScript (or any programming language), data types are different types of values you can store in a variable — like numbers, names, true/false, etc.

### Datatypes

|Datatype|Meaning|
|--------|-------|
|`string`|A string is any text — like names, words, or sentences.|
|`number`|Used for any kind of numbers — like age, marks, price, etc.|
|`boolean`|This is for true or false values — used for yes/no or on/off type situations.|
|`null`|This means nothing is inside the variable — empty on purpose|
|`undefined`|This means the variable is declared but not given any value yet.|

##  Arithmetic Operators

| Operator | Meaning             | Example  | Answer |
| -------- | ------------------- | -------- | ------ |
| `+`      | Addition            | `5 + 3`  | `8`    |
| `-`      | Subtraction         | `10 - 4` | `6`    |
| `*`      | Multiplication      | `4 * 2`  | `8`    |
| `/`      | Division            | `8 / 2`  | `4`    |
| `%`      | Remainder (modulus) | `10 % 3` | `1`    |

### code
let a = 10;
let b = 3;

console.log(a + b);  // 13<br>
console.log(a - b);  //7<br>
console.log(a * b);  // 30<br>
console.log(a / b);  // 3.33<br>
console.log(a % b);  // 1<br>

## Comparison Operators

| Operator | Meaning                  | Example     | Answer  |
| -------- | ------------------------ | ----------- | ------- |
| `==`     | Equal to                 | `5 == 5`    | `true`  |
| `===`    | Equal + same type        | `5 === '5'` | `false` |
| `!=`     | Not equal to             | `6 != 4`    | `true`  |
| `>`      | Greater than             | `8 > 4`     | `true`  |
| `<`      | Less than                | `2 < 5`     | `true`  |
| `>=`     | Greater than or equal to | `5 >= 5`    | `true`  |
| `<=`     | Less than or equal to    | `4 <= 3`    | `false` |

### code

let x = 10;
let y = 5;

console.log(x > y);    // true<br>
console.log(x < y);    // false<br>
console.log(x == 10);  // true<br>
console.log(x === "10"); // false (because different types)<br>
console.log(x != y);   // true

## Conditional statement

|statements|when to use|
|----------|-----------|
|`if`| Use if when you want to check one condition.|
|`else`|Use when you want two choices: one for true, one for false.|
|`switch`|Use when you’re checking many values of one variable|

`if`

let marks = 80;

if (marks > 35) {<br>
  console.log("You passed!");<br>
}

`else`

let marks = 30;

if (marks >= 35) {<br>
  console.log("You passed!");<br>
} else {<br>
  console.log("You failed.");<br>
}

## Loops and Functions
| Loop Type    | Use When…                         |
| ------------ | --------------------------------- |
| `for` loop   | You know how many times to repeat |
| `while` loop | You’re not sure how many times    |
| `do...while` | Want to run at least once         |
<hr>

#### write a for loop to print number's from 1-10.

`code`

for(let i= 1; i=>10; i++) {<br>
    console.log(i);<br>
}

#### create a function that returns the square of a number

`code`

function square(number) {<br>
  return number * number;<br>
}
 #### Rewrite the same function using arrow syntax

 const square = (num) => {<br>
  return num * num;<br>
};

## what is an array?

An array in JavaScript is a special variable that can store multiple values in a single variable.

Think of it like a list or a box with compartments — each compartment stores one item, and you can access them by their position 