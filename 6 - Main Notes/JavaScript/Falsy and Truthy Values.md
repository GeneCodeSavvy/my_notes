2024-08-28 18:20

Status : #mature 

Tags : [[Type Coercion]]

In JavaScript, values are classified as **truthy** or **falsy** depending on how they are evaluated in a Boolean context (e.g., in an `if` statement or a ternary operator).

## Falsy Values

A falsy value is one that translates to `false` when evaluated in a Boolean context. The following are considered falsy values in JavaScript:

1. **`false`** - The Boolean `false` value.
2. **`0`** - The number zero.
3. **`-0`** - Negative zero (uncommon, but still falsy).
4. **`""` or `''` or ````** - Empty string (single, double, or backticks).
5. **`null`** - Represents the intentional absence of any object value.
6. **`undefined`** - Indicates a variable that hasn't been assigned a value.
7. **`NaN`** - Stands for "Not-a-Number," usually the result of invalid or undefined mathematical operations.

Example:
```js
if (0) {
	 console.log("This won't run because 0 is falsy.");
	} else {     
	 console.log("This will run because 0 is falsy."); 
	}
```


## Truthy Values

A truthy value is anything that is not falsy. Essentially, any value that is not in the list of falsy values above is considered truthy.

Examples of truthy values:

- **Non-zero numbers** (e.g., `1`, `-1`, `3.14`)
- **Non-empty strings** (e.g., `"hello"`, `'0'`, `"false"`)
- **Objects** (e.g., `{}`, `[]`)
- **Functions** (e.g., `function() {}`)

Example:

```js
if (1) {
console.log("This will run because 1 is truthy.");
}
```

## **References** 
1. chatGPT
