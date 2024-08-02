Introduction to JavaScript

What is JavaScript?

## Overview of JavaScript
Use cases and where it runs (browsers, servers, etc.)
Setting Up the Development Environment

Installing Node.js
Using a text editor (e.g., VS Code)
Writing Your First JavaScript Program

Example: 
``console.log("Hello, World!");``
Basic Syntax and Variables

## Variables and Data Types

Variables: ``let``, ``const``, ``var``
<br/>
Data Types: ``Number``, ``String``, ``Boolean``, ``Null``, ``Undefined``, ``Object``, ``Symbol``
```
let age = 25; // Number
const name = "John"; // String
var isStudent = true; // Boolean
let height = null; // Null
let weight; // Undefined
```

## Basic Operators
<br/>
- Arithmetic: +, -, *, /, % <br/>
- Assignment: =, +=, -=, *=, /= <br/>
- Comparison: ==, ===, !=, !==, >, <, >=, <= <br/>
- Logical: &&, ||, !

```
let x = 10;
let y = 5;
console.log(x + y); // 15
console.log(x > y); // true
console.log(x === y); // false
```

```
let a = 10;
let b = 5;
console.log("Addition: " + (a + b)); // 15
console.log("Subtraction: " + (a - b)); // 5
console.log("Multiplication: " + (a * b)); // 50
console.log("Division: " + (a / b)); // 2
```

## Control Structures

### Conditional Statements: If-Else
```
let age = 18;
if (age >= 18) {
  console.log("You are an adult.");
} else {
  console.log("You are a minor.");
}
```

### Switch Statement
```
let day = 3;
switch (day) {
  case 1:
    console.log("Monday");
    break;
  case 2:
    console.log("Tuesday");
    break;
  case 3:
    console.log("Wednesday");
    break;
  default:
    console.log("Invalid day");
}
```
### Loops: For, While, Do-While
```
// For Loop
for (let i = 0; i < 5; i++) {
  console.log("For Loop: " + i);
}

// While Loop
let j = 0;
while (j < 5) {
  console.log("While Loop: " + j);
  j++;
}

// Do-While Loop
let k = 0;
do {
  console.log("Do-While Loop: " + k);
  k++;
} while (k < 5);
```

### Example: Number Guessing Game

```
let secretNumber = 7;
let guess = 0;

while (guess !== secretNumber) {
  guess = parseInt(prompt("Guess the number (between 1 and 10): "));
  if (guess === secretNumber) {
    console.log("Congratulations! You guessed the correct number.");
  } else {
    console.log("Try again.");
  }
}
```

## Functions
### Defining Functions
```
function greet(name) {
  return "Hello, " + name;
}
console.log(greet("Alice")); // Hello, Alice
```
### Function Parameters and Return Values
```
function add(a, b) {
  return a + b;
}
console.log(add(5, 3)); // 8
```
### Arrow Functions
```
const multiply = (a, b) => a * b;
console.log(multiply(4, 3)); // 12
```
### Example: Temperature Converter
```
function celsiusToFahrenheit(celsius) {
  return (celsius * 9/5) + 32;
}
console.log(celsiusToFahrenheit(0)); // 32
console.log(celsiusToFahrenheit(100)); // 212
```

## Arrays
### Creating and Accessing Arrays
```
let fruits = ["Apple", "Banana", "Cherry"];
console.log(fruits[0]); // Apple
```
### Array Methods: push, pop, shift, unshift, length
```
let numbers = [1, 2, 3];
numbers.push(4); // [1, 2, 3, 4]
numbers.pop(); // [1, 2, 3]
numbers.shift(); // [2, 3]
numbers.unshift(0); // [0, 2, 3]
console.log(numbers.length); // 3
```
### Example: Sum of Array Elements
```
let numbers = [1, 2, 3, 4, 5];
let sum = 0;

for (let i = 0; i < numbers.length; i++) {
  sum += numbers[i];
}

console.log("Sum: " + sum); // Sum: 15
```
