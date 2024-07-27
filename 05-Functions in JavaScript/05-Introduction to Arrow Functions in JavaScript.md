### Introduction to Arrow Functions in JavaScript

#### What We Will Learn
- The concept and syntax of arrow functions.
- Differences between traditional functions and arrow functions.

#### What are Arrow Functions?
Arrow functions, introduced in ES6 (ECMAScript 2015), offer a more concise syntax for writing functions. They are best suited for non-method functions.

#### Basic Syntax of Arrow Functions
Here's how you can define a simple arrow function:
```javascript
const greet = name => console.log(`Hello, ${name}`);
greet("Alice"); // Output: "Hello, Alice!"
```

#### Comparing Traditional Functions and Arrow Functions

**Traditional Function Expression:**
```javascript
const square = function(number) {
    return number * number;
};
console.log(square(5)); // Output: 25
```

**Arrow Function Equivalent:**
```javascript
const square = number => number * number;
console.log(square(5)); // Output: 25
```

#### Handling Multiple Parameters and No Parameters
For multiple parameters or no parameters, use parentheses:
```javascript
// Multiple parameters
const add = (a, b) => a + b;
console.log(add(2, 3)); // Output: 5

// No parameters
const logMessage = () => console.log("Logging a message");
logMessage(); // Output: "Logging a message"
```

#### Summary
- Arrow functions offer a shorter syntax for writing functions in JavaScript.
