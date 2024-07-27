### Understanding Function Return Values in JavaScript 🔄

#### What We Will Learn
- Functions with return values.
- Differences between functions that return values and those that don't.

#### Functions with Multiple Parameters 📌
Consider a function in JavaScript:
```javascript
function productOfTwoNumbers(a, b) {
    console.log(a * b);
}
productOfTwoNumbers(1, 2); // Prints 2
```

#### Functions That Do Not Return Values 🚫
The above function prints the product of `a` and `b`. If we try to store its output in a variable:
```javascript
let product = productOfTwoNumbers(1, 2); // Prints 2
console.log(product); // Prints undefined
```
Here, `product` is `undefined` because `productOfTwoNumbers` does not return a value.

#### Built-in Functions Returning a Value ✔️
Built-in JavaScript functions like `Math.max()` return a value:
```javascript
let maximum = Math.max(1, 2, 3, 4); // Stores 4 in variable maximum
console.log(maximum); // Prints 4
console.log(maximum * 5); // Prints 20
```

#### Creating a Function That Returns a Value 🔄
We can modify our function to return the product of two numbers:
```javascript
function productOfTwoNumbers(a, b) {
    return a * b;
}
console.log(productOfTwoNumbers(2, 3)); // Prints 6
```
Now, the function's result can be stored in a variable:
```javascript
let productResult = productOfTwoNumbers(2, 3); // Stores 6 in productResult
console.log(productResult); // Prints 6
console.log(productResult * 10); // Prints 60
```

#### Example: Calculating the Sum of Three Numbers 🧮
```javascript
function calculateSumOfThreeNumbers(a, b, c) {
    return a + b + c;
}
```
This function returns the sum of its three parameters.

#### Understanding the Terminology 📖
- **Function**: A block of code designed to perform a particular task. Defined using the `function` keyword.
- **Parameter**: A variable listed as part of the function's definition.
- **Argument**: The actual value passed to the function.
- **Function Declaration**: The process of defining a function's name, parameters, and body.
- **Function Invocation (or Call)**: Executing a function using its name and providing necessary arguments.
- **Return Value**: The output that a function sends back to its caller.


