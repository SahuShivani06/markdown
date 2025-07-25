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

### let,const \& var

var( The old way) before ES6: Variable can be re- declared \& updated. a global scope variable.

let( Modern way) ES6+ : Variable cannot be re - declared but can be updated. A block scope variable . 

const( Constant value): Variable cannot be re- declared or updated. A block scope variable

<hr>
1\. Primitive Data Types

Primitive data types are the built-in data types provided by JavaScript.

1\. Number:

Number data type in JavaScript can be used to hold decimal values as well as values without decimals.

Example: Below is an example.

let x = 250;

2\. String:

The string data type in JavaScript represents a sequence of characters that are surrounded by single or double quotes.

Example: Below is an example.

let fullname= "Shivani"

3\. Undefined:

This means that a variable has been declared but has not been assigned a value, or it has been explicitly set to the value `undefined`.

Example: Below is an example.

let x;

console.log(x); // Outputs: undefined

4\. Boolean:

The boolean data type can accept only two values i.e. true and false.

Example: Below is an example.

isFollow = true;

5.Null:

This data type can hold only one possible value that is null.

Example: Below is an example.

let x = null;

6\. BigInt:

BigInt data type can represent numbers greater than 253-1 which helps to perform operations on large numbers. The number is specified by writing 'n' at the end of the value

Example: Below is an example.

let x = BigInt("123");

7\. Symbol:

Symbol data type is used to create objects which will always be unique. these objects can be created using Symbol constructor.

Example:

let y = Symbol*(*Hello!);



2\. Non-Primitive datatype

1. objects :

Collection of data

It is stored as key:value

ex :

{ name: "ashok"

age:24}

note: let ko update kar sakte h

const ko nhi kar sakte

const ke object ke key ko update kar sakte h






