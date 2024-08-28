2024-08-28 18:26

Status : #mature 

Tags : [[Primitive value type]]

## **Definition**: The process of automatically converting one data type to another when operators or expressions require it.

## **Common Cases**:
  - **String Coercion**: Occurs with the `+` operator.
    - Example: `123 + "456"` → `"123456"`
  - **Number Coercion**: Occurs with arithmetic operators (`-`, `*`, `/`).
    - Example: `"10" - 2` → `8`
  - **Boolean Coercion**: Occurs in logical contexts (e.g., `if` statements).
    - Example: `if ("")` → `false` (empty string coerced to `false`)

## **Key Point**: Can lead to unexpected results, especially in comparisons.
  - Example: `1 == "1"` → `true` (loose equality with coercion)
  - Example: `1 === "1"` → `false` (strict equality, no coercion)

## Example

```js
// Type Coercion (Implicit)
let result1 = 1 + "2"; // "12" (Number coerced to String)
let result2 = "5" - 2; // 3 (String coerced to Number)
let result3 = 0 == false; // true (Boolean coerced to Number)

```
## **References** 

