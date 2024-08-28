2024-08-28 14:29

Status : #baby 

Tags : [[Datatypes]]

1. Type Conversion (Explicit Conversion)
- **Definition**: The process of explicitly converting a value from one data type to another using built-in functions.
- **Common Methods**:
  - **String Conversion**: `String()` or `.toString()`
    - Example: `String(123)` → `"123"`
  - **Number Conversion**: `Number()`, `parseInt()`, `parseFloat()`
    - Example: `Number("123")` → `123` 
    - **parseInt()**: Converts a string to an integer. 
	    - Example: `parseInt("123.45")` → `123` 
	    - Example with radix: `parseInt("101", 2)` → `5` (interprets "101" as a binary number) 
	- **parseFloat()**: Converts a string to a floating-point number. 
		- Example: `parseFloat("123.45")` → `123.45`
  - **Boolean Conversion**: `Boolean()`
    - Example: `Boolean(1)` → `true`
- **Key Point**: Controlled by the developer, making it predictable and explicit.

2. Type Coercion (Implicit Conversion)
- **Definition**: The process of automatically converting one data type to another when operators or expressions require it.
- **Common Cases**:
  - **String Coercion**: Occurs with the `+` operator.
    - Example: `123 + "456"` → `"123456"`
  - **Number Coercion**: Occurs with arithmetic operators (`-`, `*`, `/`).
    - Example: `"10" - 2` → `8`
  - **Boolean Coercion**: Occurs in logical contexts (e.g., `if` statements).
    - Example: `if ("")` → `false` (empty string coerced to `false`)
- **Key Point**: Can lead to unexpected results, especially in comparisons.
  - Example: `1 == "1"` → `true` (loose equality with coercion)
  - Example: `1 === "1"` → `false` (strict equality, no coercion)

### 3. Differences Between Type Conversion and Type Coercion
- **Type Conversion**:
  - Explicit and controlled by the developer.
  - More predictable.
- **Type Coercion**:
  - Implicit and performed automatically by JavaScript.
  - Can result in unexpected behaviour.

### 4. Examples

```js
// Type Conversion (Explicit)
let str = String(123); // "123"
let num = Number("123"); // 123
let bool = Boolean(0); // false

// Type Coercion (Implicit)
let result1 = 1 + "2"; // "12" (Number coerced to String)
let result2 = "5" - 2; // 3 (String coerced to Number)
let result3 = 0 == false; // true (Boolean coerced to Number)

```


## **References** 
1. chatGPT
