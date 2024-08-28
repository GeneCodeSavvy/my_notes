2024-08-28 14:29

Status : #baby 

Tags : [[Primitive value type]]

## **Definition**: The process of explicitly converting a value from one data type to another using built-in functions.

## **Common Methods**:
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

## **Key Point**: Controlled by the developer, making it predictable and explicit.

### 4. Examples

```js
// Type Conversion (Explicit)
let str = String(123); // "123"
let num = Number("123"); // 123
let bool = Boolean(0); // false

```

## **References** 
1. chatGPT
