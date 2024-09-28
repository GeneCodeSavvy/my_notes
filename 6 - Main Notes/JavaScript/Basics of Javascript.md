2024-07-27 16:02

Status : #baby

Tags : [[How the Browser Works]]




>[!SUMMARY]- Table of Contents
```table-of-contents
style: nestedOrderedList
```

# What is JavaScript ?

JavaScript is a high-level, dynamic, and interpreted programming language that is primarily used for enhancing the interactivity of web pages. It allows developers to create dynamically updating content, control multimedia, animate images, and pretty much everything else. It is a core technology of the World Wide Web, alongside HTML and CSS.

# Data Types in JavaScript

JavaScript can store information in the following data types:
1. `undefined` - A variable that has not been assigned a value.
2. `null` - Represents the intentional absence of any object value.
3. `boolean` - Represents a logical entity and can have two values: `true` or `false`.
4. `string` - Used for textual data. Enclosed in single (`'`) or double (`"`) quotes.
5. `number` - Represents both integer and floating-point numbers.
6. `object` - Used to store collections of data and more complex entities. 


# Declaring Variables in JavaScript

In JavaScript, variables can be declared using three keywords: `var`, `let`, and `const`.

1. `var`
   - Function-scoped.
   - Can be re-declared and updated.
   
2. `let`
   - Block-scoped.
   - Can be updated but not re-declared within the same scope.
   
3. `const`
   - Block-scoped.
   - Cannot be updated or re-declared.


# Initialising Variables in JavaScript

Initialising a variable means assigning it a value at the time of declaration. Remember that variable name are case sensitive.
1. Using `var`
```javascript
var a = 1;
```

2. Using `let`
```javascript
let b = 2;
```

3. Using `const`
```javascript
const c = 3;
```



# Logical Operators in JavaScript

1. AND operator - &&
2. OR operator - ||
3. NOT operator - !


# Mathematical Operators in JavaScript 

1. Addition : +
2. Subtraction : - 
3. Multiplication : *
4. Division : /


# Comparison Operators in JavaScript

1. greater than : >
2. smaller than: <
3. equal : ==


# Increment and Decrement Operators in JavaScript

**Increment Operator (`++`)**
The increment operator increases the value of a variable by one. It can be used in two forms:
1. **Prefix Increment (`++variable`)**: Increments the value before it is used in an expression.
2. **Postfix Increment (`variable++`)**: Increments the value after it is used in an expression.

**Decrement Operator (`--`)**
The decrement operator decreases the value of a variable by one. It also has two forms:
1. **Prefix Decrement (`--variable`)**: Decrements the value before it is used in an expression.
2. **Postfix Decrement (`variable--`)**: Decrements the value after it is used in an expression.


# Augmented Math Operations in JavaScript

**Definition:** Augmented math operations are shorthand operators that combine arithmetic operations with assignment.

**Operators**:
- `+=`: Adds and assigns the result.
- `-=`: Subtracts and assigns the result.
- `*=`: Multiplies and assigns the result.
- `/=`: Divides and assigns the result.
- `%=`: Computes the remainder and assigns the result.
- `**=`: Raises to a power and assigns the result (ES6).


# Escape Sequences in JavaScript

- **Purpose**: Escape sequences are used to represent special characters in strings that are difficult to include directly.
- **Common Escape Sequences**:
  - `\n` : Newline
  - `\r` : Carriage return
  - `\t` : Horizontal tab
  - `\b` : Backspace
  - `\f` : Form feed
  - `\\` : Backslash
  - `\'` : Single quote
  - `\"` : Double quote
  - `\uXXXX` : Unicode character (where XXXX is the 4-digit hexadecimal code)
  - `\xXX` : ASCII character (where XX is the 2-digit hexadecimal code)

# Array Manipulation in JavaScript

https://www.freecodecamp.org/news/manipulating-arrays-in-javascript/


# Functions in JavaScript 

It is a reusable block of code, that can be called anytime in the codebase.

[[How the Browser Works]]