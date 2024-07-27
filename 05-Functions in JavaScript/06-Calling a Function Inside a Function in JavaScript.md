### Calling a Function Inside a Function in JavaScript

#### What We Will Learn
- The concept of calling a function inside another function.
- Practical examples of nested function calls.
- Benefits of using nested functions.

#### Why Call a Function Inside a Function?
Calling a function inside another function allows for code reuse, modularity, and separation of concerns. It helps in organizing code and making it more maintainable.

#### Basic Example of Nested Function Calls
Let's start with a simple example where we have two functions: one to calculate the square of a number and another to calculate the sum of the squares of two numbers.

**Function to Calculate Square:**
```javascript
const square = number => number * number;
console.log(square(5)); // Output: 25
```

**Function to Calculate Sum of Squares:**
```javascript
const sumOfSquares = (a, b) => {
    return square(a) + square(b);
};
console.log(sumOfSquares(2, 3)); // Output: 13
```

Here, the `sumOfSquares` function calls the `square` function for both its parameters.

#### Building a User Access System
Let's use nested functions to build a simple user access system with the following functionality:
- Check if the user is logged in.
- Check if the logged-in user has access to a specific resource.

**Function to Check User Login:**
```javascript
const isUserLoggedIn = user => {
    return user !== null && user !== undefined;
};
```

**Function to Check User Access:**
```javascript
const hasAccess = user => {
    if (isUserLoggedIn(user)) {
        return user.role === 'admin' || user.role === 'editor';
    }
    return false;
};
```

**Using the Functions:**
```javascript
let user1 = { name: "Alice", role: "admin" };
let user2 = { name: "Bob", role: "viewer" };
let user3 = null;

console.log(hasAccess(user1)); // Output: true
console.log(hasAccess(user2)); // Output: false
console.log(hasAccess(user3)); // Output: false
```

In this example:
- `isUserLoggedIn` is called inside `hasAccess` to check if the user is logged in.
- `hasAccess` then checks the user's role to determine if they have access.

#### Benefits of Nested Functions
- **Code Reuse**: Functions can be reused within other functions without duplicating code.
- **Modularity**: Breaks down complex problems into smaller, manageable functions.
- **Separation of Concerns**: Each function can focus on a single task, improving readability and maintainability.


---

Happy coding! 🚀💻