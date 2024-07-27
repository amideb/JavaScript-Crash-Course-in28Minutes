### Exploring Functions with Parameters in JavaScript 🌐

#### What We Will Learn
- The power of parameters in functions.
- Creating and using functions with parameters.

#### The Power of Parameters in Functions 💡
Parameters enable functions to perform operations using different input values, enhancing their reusability and functionality.

#### Creating a Function with a Parameter 🔧
Here's a simple function that takes a parameter:
```javascript
function greet(name) {
    console.log("Hello, " + name);
}
```
In this function, `name` is a parameter that the function uses to customize the greeting.

#### Calling a Function with an Argument 📞
When invoking the function, you provide an argument that replaces the parameter:
```javascript
greet("Alice"); // Output: Hello, Alice
greet("Bob");   // Output: Hello, Bob
```
Each time `greet` is called with a different argument, it outputs a personalized message.

#### Hello World with a Parameter 🌍
Extending the "Hello World" example to include a parameter:
```javascript
function printHelloWorld(times) {
    for (let i = 1; i <= times; i++) {
        console.log("Hello World");
    }
}
```
This function now accepts a `times` parameter, determining how many times "Hello World" is printed.

#### Calling Hello World Function 📬
Invoke the function with different numbers:
```javascript
printHelloWorld(1); // Prints "Hello World" once
printHelloWorld(3); // Prints "Hello World" three times
```

#### Simple Yet Powerful 🚀
Using parameters in functions opens up numerous possibilities, allowing the same function to perform various tasks based on the input provided.

#### Remember 📘
- Parameters greatly enhance the flexibility of functions.
- Always use meaningful names for parameters to make your code clear.
- Experiment with different arguments to see how they affect your function's behavior.
