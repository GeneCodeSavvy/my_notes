2024-08-30 13:38

Status : #mature 

Tags : [[Expression Statements]]

---
## Overview
A function expression is another way to define a function, where the function is defined as part of an expression, typically by assigning it to a variable. Unlike function declarations, function expressions do not have names (when anonymous) and are not hoisted, giving you more control over when and how the function is created and invoked.

## Syntax
A function expression consists of the `function` keyword, optionally followed by a name (if it's a named function expression), a list of parameters, and a function body.

```javascript
const variableName = function(parameter1, parameter2, ...) {
    // Function body
};
```

## Example:
```javascript
const greet = function(name) {
    console.log("Hello, " + name + "!");
};

greet("Harsh");  // Output: "Hello, Harsh!"
```
In this example, the function is assigned to the variable `greet`. The function can then be invoked using this variable.

## Key Characteristics
1. **Anonymous Functions:**
   - Function expressions are often **anonymous**, meaning they do not have a name. However, you can also create named function expressions.
   - Example:
   ```javascript
   const sayHello = function() {
       console.log("Hello!");
   };
   ```

2. **Named Function Expressions:**
   - Although uncommon, you can give a function expression a name. This can be useful for recursion or for debugging purposes.
   - Example:
   ```javascript
   const factorial = function fact(n) {
       return (n <= 1) ? 1 : n * fact(n - 1);
   };

   console.log(factorial(5));  // Output: 120
   ```

3. **No Hoisting:**
   - Unlike function declarations, function expressions are not hoisted. This means that the function cannot be called before it is defined.
   - Example:
   ```javascript
   sayHi();  // Error: sayHi is not defined

   const sayHi = function() {
       console.log("Hi!");
   };
   ```

4. **Assigned to Variables or Properties:**
   - Function expressions can be assigned to variables, properties of objects, or even elements of arrays.
   - Example:
   ```javascript
   const obj = {
       greet: function() {
           console.log("Hello from the object!");
       }
   };
   obj.greet();  // Output: "Hello from the object!"
   ```

5. **Used as Callbacks:**
   - Function expressions are frequently used as **callback functions**, passed as arguments to other functions.
   - Example:
   ```javascript
   setTimeout(function() {
       console.log("This runs after 2 seconds");
   }, 2000);
   ```

6. **IIFE (Immediately Invoked Function Expressions):**
   - A function expression can be immediately executed upon creation by wrapping it in parentheses and adding `()` at the end. This is known as an **Immediately Invoked Function Expression (IIFE)**.
   - Example:
   ```javascript
   (function() {
       console.log("This function runs immediately!");
   })();
   ```

## Advantages of Function Expressions
1. **Flexible Placement:** Function expressions can be defined and passed around as values, making them ideal for use in callbacks, event handlers, and more.
2. **Encapsulation:** IIFEs are commonly used to encapsulate code, creating private scopes that help prevent variable collisions.
3. **Conditional Definition:** You can define a function based on a condition, which can be useful in certain situations.

## Use Cases
1. **Callbacks:**
   Function expressions are commonly used as callbacks for asynchronous operations or event handling.
   ```javascript
   document.addEventListener('click', function() {
       console.log("Document clicked!");
   });
   ```

2. **Creating Closures:**
   Function expressions allow you to create closures, where an inner function has access to the outer function's scope.
   ```javascript
   function outerFunction() {
       let count = 0;
       return function() {
           count++;
           console.log(count);
       };
   }
   const increment = outerFunction();
   increment();  // Output: 1
   increment();  // Output: 2
   ```

3. **Dynamic Function Definition:**
   Function expressions can be conditionally defined based on runtime logic.
   ```javascript
   let greet;
   if (userIsAdmin) {
       greet = function() { console.log("Welcome, Admin!"); };
   } else {
       greet = function() { console.log("Welcome, User!"); };
   }
   greet();
   ```

## Limitations
- **Not Hoisted:** Since function expressions are not hoisted, they must be defined before they can be used.
- **Less Readable:** If overused, anonymous function expressions can make code less readable and harder to debug.

## Conclusion
Function expressions offer flexibility and control over how functions are defined and used in JavaScript. Whether you need to define a callback, create an IIFE, or encapsulate logic within a closure, function expressions are a powerful tool in modern JavaScript development.

## **References** 

