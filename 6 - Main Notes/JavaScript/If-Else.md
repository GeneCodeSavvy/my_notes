2024-08-28 20:25

Status : #mature 

Tags : [[Conditional Statements]]

### JavaScript `if-else` Statements
---
## **Overview:**

The `if-else` statement in JavaScript is used to execute a block of code based on a condition. It allows for conditional execution, which means different blocks of code will run depending on whether a condition evaluates to `true` or `false`.

## Basic Syntax:

```javascript
if (condition) {
  // Code to be executed if the condition is true
} else {
  // Code to be executed if the condition is false
}
```

**Explanation:**

1. **Condition:** The expression inside the parentheses `(condition)` is evaluated. If it returns `true`, the code inside the first block `{ ... }` is executed.
2. **Else Block:** If the condition returns `false`, the code inside the `else` block is executed.

## Example:

```javascript
let temperature = 25;

if (temperature > 30) {
  console.log("It's hot outside!");
} else {
  console.log("The weather is pleasant.");
}
```

In this example:
- If the `temperature` is greater than 30, the message "It's hot outside!" is printed.
- Otherwise, the message "The weather is pleasant." is printed.

## `else if` Clause:

The `else if` clause allows you to check multiple conditions in sequence. It provides more flexibility by chaining multiple conditions together.

**Syntax:**

```javascript
if (condition1) {
  // Code to be executed if condition1 is true
} else if (condition2) {
  // Code to be executed if condition1 is false and condition2 is true
} else {
  // Code to be executed if both condition1 and condition2 are false
}
```

**Example:**

```javascript
let score = 85;

if (score >= 90) {
  console.log("Grade: A");
} else if (score >= 80) {
  console.log("Grade: B");
} else if (score >= 70) {
  console.log("Grade: C");
} else {
  console.log("Grade: D");
}
```

Here:
- If the score is 90 or above, the grade "A" is printed.
- If the score is between 80 and 89, the grade "B" is printed.
- If the score is between 70 and 79, the grade "C" is printed.
- Otherwise, the grade "D" is printed.

## Nesting `if-else` Statements:

You can nest `if-else` statements inside each other to check more complex conditions. This involves placing an `if-else` statement inside another `if-else` statement.

**Example:**

```javascript
let age = 20;
let hasTicket = true;

if (age >= 18) {
  if (hasTicket) {
    console.log("You can enter the concert.");
  } else {
    console.log("You need a ticket to enter.");
  }
} else {
  console.log("You must be at least 18 years old to enter.");
}
```

In this example:
- The first `if` checks if the person is 18 or older.
- Inside this block, another `if-else` checks if the person has a ticket.

## Ternary Operator (Shorthand for `if-else`):

The ternary operator is a shorter way of writing an `if-else` statement.

**Syntax:**

```javascript
condition ? expressionIfTrue : expressionIfFalse
```

**Example:**

```javascript
let isMember = true;
let fee = isMember ? "$10" : "$20";

console.log(fee); // Outputs "$10" if isMember is true, otherwise "$20"
```

Here, if `isMember` is `true`, the `fee` is set to "$10". If `isMember` is `false`, the `fee` is set to "$20".


## **References** 

