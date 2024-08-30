2024-08-29 19:52

Status : #mature 

Tags : [[Operators]]

---

Used as a concise alternative to an `if-else` statement.

The **ternary operator** consists of three parts:
1. A condition.
2. An expression to execute if the condition is true.
3. An expression to execute if the condition is false.

# Syntax:

```javascript
condition ? expressionIfTrue : expressionIfFalse;
```

## Example:

```javascript
let age = 20;
let message = age >= 18 ? "Adult" : "Minor";
console.log(message);  // Output: "Adult"
```

In this example, the ternary operator checks if `age` is 18 or more. If true, it returns `"Adult"`; otherwise, it returns `"Minor"`.

## Nesting Ternary Operators:
You can nest ternary operators, but this can make your code harder to read:

```javascript
let age = 20;
let category = age >= 18 ? (age >= 65 ? "Senior" : "Adult") : "Minor";
console.log(category);  // Output: "Adult"
```

In this case, the ternary operator determines if the person is a "Senior," "Adult," or "Minor."

**Note:** While ternary operators are useful for concise expressions, they should be used sparingly to maintain code readability.
## **References** 

