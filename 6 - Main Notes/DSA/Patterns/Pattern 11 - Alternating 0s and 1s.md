2024-09-23 01:37

Status : #mature 

Tags : [[Given an integer 'n' recreate a specific pattern.]]

---
## Code (JavaScript)

```javascript
class Solution {
    pattern11(n) {
        for (let i = 1; i <= n; i++) {
            if (i % 2 != 0) {
                process.stdout.write('1 ')
                for (let j = 1; j < i/2; j++) {
                    process.stdout.write('0 1 ')
                }
            } else {
                for (let j = 0; j < i/2; j++) {
                    process.stdout.write('0 1 ')
                }
            }
            console.log()
        }
    }
}
```

## Summary of Approach

This solution uses nested loops to generate a pattern of alternating 0s and 1s. The outer loop iterates through rows, while the inner loop handles the alternating pattern. The approach distinguishes between odd and even rows, starting odd rows with '1' and even rows with '0'. It uses `process.stdout.write()` to print without line breaks and `console.log()` to move to the next line.

## Pseudo Code

```pseudo
For each row from 1 to n:
    If row is odd:
        Print '1 '
        For (row - 1) / 2 times:
            Print '0 1 '
    Else:
        For row / 2 times:
            Print '0 1 '
    Move to next line
```

## Time and Space Complexity Analysis

- Time Complexity: O(n^2), where n is the input number. The nested loops result in quadratic time complexity.
- Space Complexity: O(1), as it uses a constant amount of extra space regardless of input size.

## Edge Cases Considered

- The solution handles the case when n = 1, printing just a single '1'.
- It correctly handles all positive integer inputs for n.

## Optimization Potential

The current solution is relatively optimized. However, to improve readability and potentially performance, we could:
1. Use string concatenation instead of multiple `process.stdout.write()` calls.
2. Precalculate the '0 1 ' string for repeated use.

## Visualization Aid

Here's a visual representation of how the pattern evolves for n = 5:

```
1
0 1
1 0 1
0 1 0 1
1 0 1 0 1
```

Each line represents one iteration of the outer loop, showing how 0s and 1s are alternately added to create the pattern.

---
## **References** 

