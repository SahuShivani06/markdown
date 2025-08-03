#### 1. Find the second largest number in an array.
 let numbers=[111,1587,6,72];

let max = Math.max(...numbers);

let withoutMax = numbers.filter(num => num !== max);

let secondLargest = Math.max(...withoutMax);

console.log(secondLargest); 

#### 2.  Check if two strings are anagrams.
function isAnagram(str1, str2) {
  
  str1 = str1.replace(/\s/g, '').toLowerCase();<br>
  str2 = str2.replace(/\s/g, '').toLowerCase();

 
  return str1.split('').sort().join('') === str2.split('').sort().join('');
}

console.log(listen,silent);

#### 3. Remove all falsy values from an array.

let mixedArray = [0, "hello", false, "", 42, null, undefined, NaN, "world"];

let truthyArray = mixedArray.filter(Boolean);

console.log(truthyArray);

#### 4. Flatten a nested array (1 level).

let nestedArray = [1, 2, [3, 4], 5, [6, 7]];

let flattened = nestedArray.flat();

console.log(flattened);

#### 5. Frequency count of elements in an array.
let items = ["apple", "banana", "apple", "orange", "banana", "apple"];

let frequency = {};

for (let item of items) {<br>
  frequency[item] = (frequency[item] || 0) + 1;
}

console.log(frequency);

#### 6. Destructure an object and rename a key.
object

let student = {

  fullName: "shivani",

  age: 19,

  grade: "14th"

};

destructure

let { fullName: name, age, grade } = student;

console.log(name);   
console.log(age);<br>
console.log(grade);  

#### 7. Merge two objects using the spread operator.

let obj1 = { name: "shivani"};<br>
let obj2 = { age: 18  };

let mergedObj = { ...obj1, ...obj2 };

console.log(mergedObj);

#### 8. Swap keys and values in an object.

let original = {
  name: "shivani",
  age: "19",
  grade: "14th"
};

let swapped = {};

for (let key in original) {
  swapped[original[key]] = key;
}

console.log(swapped);

 #### 9. Create a closure-based function call counter.

 function createCounter() {<br>
  let count = 0;

  return function() {
    count++;
    console.log(`Called ${count} time(s)`);
  };
}

let counter = createCounter();

counter(); 
counter(); 
counter(); 

#### 10. Function that runs only once.

function greet() {
  console.log("Hello, this runs only once!");
}

let greetOnce = runOnce(greet);

greetOnce();  
greetOnce(); 

#### 11. Function currying (e.g., add(2)(3)).

function add(a) {<br>
  return function(b) {<br>
    return a + b;<br>
  };
}

console.log(add(2)(3)); 

#### 12. Difference between var, let, and const.
| Feature       | `var`             | `let`       | `const`     |
| ------------- | ----------------- | ----------- | ----------- |
| Scope         | Function          | Block       | Block       |
| Re-declarable | ✅ Yes             | ❌ No        | ❌ No        |
| Re-assignable | ✅ Yes             | ✅ Yes       | ❌ No        |
| Hoisting      | ✅ Yes (undefined) | ✅ Yes (TDZ) | ✅ Yes (TDZ) |

#### 13. Convert a regular function to an arrow function.
function add(a, b) {<br>
  return a + b;<br>
}

const add = (a, b) => a + b;

#### 14. Use template literals for a greeting message.

let name = "Ayaan";<br>
let message = `Hello, ${name}! Welcome to the class.`;

console.log(message);