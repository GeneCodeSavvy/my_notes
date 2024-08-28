2024-08-26 19:18

Status : #mature 

Tags : [[Declarative Statements]]

These keywords are used for declaring variables in JavaScript.

1. **var Keyword**
   1. The variable value can be changed after initialisation.
   2. Variables declared with `var` are function-scoped, meaning they are accessible within the function they are declared in.
   3. `var` allows for re-declaration of the same variable within the same scope.
   4. Variables declared with `var` are hoisted, meaning they are moved to the top of their scope, but they are initialised with `undefined` until the assignment.
   
```js
function test() {
    var z = 30;
    if (true) {
        var z = 40; // This redeclares 'z' within the same function scope
        console.log(z); // 40
    }
    console.log(z); // 40
}
test();
```

2. **let Keyword**
   1. The variable value can be changed after initialisation.
   2. Variables declared with `let` are block-scoped, meaning they are accessible only within the block they are declared in (e.g., inside a loop or if statement).
   3. `let` does not allow re-declaration within the same scope, preventing accidental overwriting of variables.
   4. Variables declared with `let` are hoisted but are not initialised, meaning they remain in a "temporal dead zone" until they are assigned a value.

```js
let x = 10;
let x = 20; // Error: Identifier 'x' has already been declared

console.log(y); // Error: Cannot access 'y' before initialization
let y = 15;
```

3. **const Keyword**
   1. The variable value cannot be changed after initialisation (i.e., `const` creates a constant).
   2. JS throws an error if the value is not assigned during initialisation.
   3. Variables declared with `const` are also block-scoped, similar to `let`.
   4. While `const` prevents reassignment of the variable itself, if the variable holds an object or array, the properties or elements can still be modified.
```js
const a = 50;
a = 60; // Error: Assignment to constant variable

const b; // Error: Missing initializer in const declaration
b = 25;

const c = 70;
const c = 80; // Error: Identifier 'c' has already been declared
```


## **References** 
1. [The Complete JavaScript Course 2024: From Zero to Expert!](https://www.udemy.com/course/the-complete-javascript-course/)
2. ChatGPT

