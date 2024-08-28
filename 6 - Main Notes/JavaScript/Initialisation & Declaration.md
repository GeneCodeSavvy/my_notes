2024-08-26 19:37

Status : #mature

Tags : [[Expression Statements]] [[Declarative Statements]]

1. **Declaration**
   1. Declaration is the process of creating a variable without assigning it a value.
   2. Syntax: `var x;`, `let y;`, `const z;`
   3. Declaring a variable sets up a name in the memory, but no value is assigned to it yet.
   4. Variables declared with `var` are automatically initialized to `undefined`. However, variables declared with `let` and `const` are not initialized until a value is assigned.
   5. Variables declared with `const` must be initialized at the time of declaration.

2. **Initialization**
   1. Initialization is the process of assigning a value to a variable.
   2. Syntax: `var x = 10;`, `let y = 'Hello';`, `const z = [1, 2, 3];`
   3. Initialization can occur at the time of declaration or later in the code, except for variables declared with `const` which must be initialized at the time of declaration.
   4. Once initialized, variables declared with `let` and `var` can have their values reassigned. However, variables declared with `const` cannot be reassigned (though the contents of objects/arrays declared with `const` can be modified).
   5. Initialization of variables declared with `var` happens after hoisting, meaning that the declaration is hoisted to the top, but the initialization occurs where it is defined in the code.

### Example:

```js
// Declaration without initialization
var a;
let b;

// Declaration with initialization
var c = 10;
let d = "Hello";
const e = [1, 2, 3];

// Assigning values (initialization) after declaration
a = 5;
b = "World";

let y;  // Declaration statement (no initialization)
y = 10;  // Expression statement (initialization)

```

## **References** 