2024-08-30 06:59

Status : #mature 

Tags : [[Core language Constructs]]

---
## Overview
The `'use strict'` directive in JavaScript enforces a stricter parsing and error handling mode. This helps developers write safer, cleaner code by catching common coding mistakes and preventing potentially problematic syntax.

## Syntax

To enable strict mode, place the following directive at the beginning of your script or function:
```javascript
'use strict';
```
- **Global Strict Mode:** Place `'use strict';` at the top of your script file to enable strict mode globally.
- **Function-Level Strict Mode:** Place `'use strict';` at the beginning of a function to enable strict mode only within that function.

## Example

```javascript
'use strict';

function example() {
    x = 10;  // This will throw an error because 'x' is not declared
}

example();
```
In this example, the assignment to `x` without declaring it using `var`, `let`, or `const` will throw an error in strict mode, whereas it would have silently created a global variable in non-strict mode.

## Benefits of Using Strict Mode
1. **Prevents Accidental Globals:**
   - Variables must be declared before use. Without strict mode, assigning a value to an undeclared variable creates a global variable, which can lead to bugs.
   - Example:
   
   ```javascript
   'use strict';
   x = 10;  // Throws an error
   ```

2. **Eliminates `this` Coercion:**
   - In non-strict mode, `this` can be coerced into the global object in certain situations (e.g., within functions). Strict mode ensures that `this` remains `undefined` in such cases.
   - Example:
   
   ```javascript
   'use strict';
   function example() {
       console.log(this);  // Logs 'undefined' instead of the global object
   }
   example();
   ```

3. **Disallows Duplicate Parameter Names:**
   - In strict mode, functions cannot have duplicate parameter names, which helps prevent confusion and potential errors.
   - Example:
   
   ```javascript
   'use strict';
   function example(a, a) {  // Throws an error
       return a;
   }
   ```

4. **Disables `with` Statement:**
   - The `with` statement, which can make code harder to understand and debug, is not allowed in strict mode.
   - Example:
   
   ```javascript
   'use strict';
   with (Math) {  // Throws an error
       console.log(PI);
   }
   ```

5. **Throws Errors for Writing to Read-Only Properties:**
   - In strict mode, trying to assign a value to a non-writable property or setting a property on a primitive value will throw an error, whereas non-strict mode would silently ignore it.
   - Example:
   
   ```javascript
   'use strict';
   const obj = {};
   Object.defineProperty(obj, 'prop', { value: 42, writable: false });
   obj.prop = 10;  // Throws an error
   ```

#### Use Cases
- **Preventing Common Mistakes:** Strict mode helps avoid common coding mistakes, especially for beginners or when working on larger projects.
- **Improving Performance:** Some JavaScript engines can optimize strict mode code better than non-strict mode code, as it eliminates some ambiguous behaviors.
- **ES6 Modules:** In ES6 (ECMAScript 2015) and later, strict mode is enabled by default in modules.

#### Conclusion
The `'use strict'` directive is a useful tool for writing more reliable and predictable JavaScript code. By catching common errors and enforcing better coding practices, it can help reduce bugs and improve code quality.

---
## **References** 

