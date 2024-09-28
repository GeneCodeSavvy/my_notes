2024-09-23 02:25

Status : #mature 

Tags : [[Given an integer 'n' recreate a specific pattern.]]

---
## Question

Given an integer n. You need to recreate the pattern given below for any value of N. Let's say for N = 5, the pattern should look like as below:

```
1        1
12      21
123    321
1234  4321
1234554321
```

## Code (JavaScript)

```javascript
class Solution {
    pattern12(n) {
        for (let i = 1; i <= n; i++) {
            for (let j = 1; j <= i; j++) {
                process.stdout.write(j.toString())
            }
            for (let k = 1; k <= 2*(n - i); k++) {
                process.stdout.write(" ")
            }
            for (let l = i; l >= 1; l--) {
                process.stdout.write(l.toString())
            }
            console.log()
        }
    }
}
```

## Summary of Approach

This solution uses nested loops to generate a symmetric number pyramid pattern. The outer loop iterates through rows, while three inner loops handle different parts of each row: ascending numbers, spaces, and descending numbers. It creates a mirror effect by printing numbers in ascending order, then spaces, and finally the same numbers in descending order.

## Pseudo Code

```pseudo
For each row from 1 to n:
    Print numbers from 1 to current row
    Print spaces: 2 * (n - current row)
    Print numbers from current row to 1
    Move to next line
```

## Time and Space Complexity Analysis

- Time Complexity: O(n^2), where n is the input number. The nested loops result in quadratic time complexity.
- Space Complexity: O(1), as it uses a constant amount of extra space regardless of input size.

## Edge Cases Considered

- The solution handles the case when n = 1, printing just "11".
- It correctly handles all positive integer inputs for n.

## Optimization Potential

The current solution is relatively optimized for its approach. However, potential improvements could include:
1. Combining the first and third inner loops to reduce code duplication.
2. Using string concatenation instead of multiple `process.stdout.write()` calls, which might be more efficient for larger inputs.

## Visualization Aid

Here's a visual representation of how the pattern evolves for n = 5:

```
1        1
12      21
123    321
1234  4321
1234554321
```

Each line represents one iteration of the outer loop, showing:
- Ascending numbers (left side)
- Spaces (middle)
- Descending numbers (right side)

The pattern forms a symmetric pyramid with numbers increasing towards the center and then decreasing, while the number of spaces reduces in each row.

---
## **References** 

