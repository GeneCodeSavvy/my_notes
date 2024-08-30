2024-08-29 18:47

Status : #mature 

Tags : [[Conditional Statements]]

---
## **Overview:**

The `switch` statement in JavaScript is used to execute one block of code from multiple options based on the value of an expression. It provides a cleaner and more readable alternative to writing multiple `if-else` conditions when dealing with many possible values for a single expression.

#### Basic Syntax:

```javascript
switch (expression) {
  case value1:
    // Code to be executed if expression === value1
    break;
  case value2:
    // Code to be executed if expression === value2
    break;
  // You can add more cases here
  default:
    // Code to be executed if no case matches
}
```

**Explanation:**

1. **Expression:** The `expression` is evaluated once, and its value is compared against the values of each `case`.
2. **Case:** If the `expression` matches a `case` value, the corresponding block of code is executed.
3. **Break:** The `break` statement is used to exit the `switch` statement. Without `break`, the code execution will continue to the next case, even if it doesn’t match (known as "fall-through").
4. **Default:** The `default` case is optional and executes if none of the `case` values match the `expression`. Think of it as a fallback or else clause.

#### Example:

```javascript
let day = 3;
let dayName;

switch (day) {
  case 1:
    dayName = "Monday";
    break;
  case 2:
    dayName = "Tuesday";
    break;
  case 3:
    dayName = "Wednesday";
    break;
  case 4:
    dayName = "Thursday";
    break;
  case 5:
    dayName = "Friday";
    break;
  case 6:
    dayName = "Saturday";
    break;
  case 7:
    dayName = "Sunday";
    break;
  default:
    dayName = "Invalid day";
}

console.log(dayName); // Outputs "Wednesday"
```

In this example:
- The `switch` statement checks the value of `day`.
- When `day` equals 3, the block of code under `case 3` is executed, assigning `"Wednesday"` to `dayName`.
- The `break` statement ensures the code doesn’t fall through to subsequent cases.

## Using Multiple Cases for the Same Code:

You can group multiple cases together if they should execute the same code.

**Example:**

```javascript
let fruit = "apple";

switch (fruit) {
  case "apple":
  case "pear":
    console.log("This is a type of pome fruit.");
    break;
  case "orange":
  case "lemon":
    console.log("This is a type of citrus fruit.");
    break;
  default:
    console.log("Unknown fruit type.");
}
```

In this example:
- The cases for `"apple"` and `"pear"` are grouped together since they share the same output.
- Similarly, `"orange"` and `"lemon"` share the same output.

## Omitting `break` (Fall-through):

If you omit the `break` statement, the code execution will continue into the next case, even if the next case doesn’t match the expression. This behavior is known as "fall-through."

**Example:**

```javascript
let score = 75;

switch (true) {
  case score >= 90:
    console.log("Grade: A");
    break;
  case score >= 80:
    console.log("Grade: B");
    break;
  case score >= 70:
    console.log("Grade: C");
    // No break here, so it will fall through
  case score >= 60:
    console.log("Grade: D");
    break;
  default:
    console.log("Grade: F");
}
```

In this example:
- If `score` is 75, both "Grade: C" and "Grade: D" will be printed because there’s no `break` after the `case score >= 70`.

## Best Practices with `switch`:

1. **Always Use `break`:** Ensure each `case` ends with a `break` statement unless you specifically want the code to fall through to the next case.
2. **Default Case:** Always include a `default` case to handle unexpected values of the expression.
3. **Readability:** Use `switch` when you have multiple conditions based on the same expression for better readability compared to multiple `if-else` statements.

## **References** 

