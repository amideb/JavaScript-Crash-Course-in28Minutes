### Default Function Arguments in JavaScript 🌟

#### What We Will Learn
- Understanding default function arguments.
- Creating functions with default parameters.

#### Function Without Default Arguments
First, let's define a function `printString` that takes two parameters: `str` and `numberOfTimes`. It prints `str` `numberOfTimes` times.
```javascript
function printString(str, numberOfTimes) {
    for (let i = 0; i < numberOfTimes; i++) {
        console.log(str);
    }
}
// Calling the function with both arguments
printString("Hello World", 3); // Outputs "Hello World" three times
```
If you call this function with just one argument, it won't work as expected because JavaScript will set `numberOfTimes` to `undefined`.

#### Introducing Default Arguments
Now, let's add default values to the parameters:
```javascript
function printString(str = "Hello World", numberOfTimes = 5) {
    for (let i = 0; i < numberOfTimes; i++) {
        console.log(str);
    }
}
// Calling the function without any arguments
printString(); // Outputs "Hello World" five times
```
With default arguments, the function becomes more versatile:
- Call without any arguments: uses default values.
- Call with one argument: overrides the first parameter, second remains default.
- Call with both arguments: uses provided values.

#### Examples of Different Calls 📞
```javascript
// With one custom argument
printString("Welcome to JavaScript"); // Outputs "Welcome to JavaScript" five times

// With both arguments
printString("Welcome to JavaScript", 3); // Outputs "Welcome to JavaScript" three times
```

#### Remember 📘
- Default arguments in functions provide flexibility, allowing functions to operate even when some arguments are not provided.
- This feature is handy for setting common default values and accommodating various use cases with a single function definition.
