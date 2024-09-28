2024-09-23 21:24

Status : #mature 

Tags : [[Given an integer 'n' recreate a specific pattern.]]

---
## Question 

Given an integer n. You need to recreate the pattern given below for any value of N. Let's say for N = 5, the pattern should look like as below:
  
```markdown
1 

2 3 

4 5 6 

7 8 9 10 

11 12 13 14 15
```

## Code (JavaScript)

```javascript
class Solution {
    pattern13(n) {
        let num = 1
        for (let i = 1; i <= n; i++) {
            for (let j = 1; j <= i; j++) {
                process.stdout.write(num + " ")
                num++
            }
            console.log()
        }
    }
}
```

## Summary of Approach

This solution uses nested loops to generate a triangle pattern of increasing numbers. The outer loop represents rows, while the inner loop prints numbers in each row. A single variable `num` keeps track of the current number to be printed, incrementing after each use. This approach ensures a continuous sequence of numbers across all rows, creating a triangle pattern where each row contains one more number than the previous.

## Pseudo Code

```pseudo
Initialize num = 1
For each row from 1 to n:
    For each column from 1 to current row number:
        Print num followed by a space
        Increment num
    Move to next line
```

## Time and Space Complexity Analysis

- Time Complexity: O(n^2), where n is the input number. The nested loops result in a total of n(n+1)/2 iterations.
- Space Complexity: O(1), as it uses a constant amount of extra space regardless of input size.

## Edge Cases Considered

- The solution handles the case when n = 1, printing just "1".
- It correctly handles all positive integer inputs for n.

## Optimization Potential

The current solution is already well-optimized for its purpose. However, for very large inputs, potential improvements could include:
1. Using string concatenation instead of multiple `process.stdout.write()` calls.
2. If memory isn't a concern, pre-generating the entire pattern as a string before printing.

## Visualization Aid

Here's a visual representation of how the pattern evolves for n = 5:

```
1 
2 3 
4 5 6 
7 8 9 10 
11 12 13 14 15
```

Each line represents one iteration of the outer loop, showing:
- The number of elements in each row increases by 1
- Numbers continue sequentially across rows
- The pattern forms a right-angled triangle

---
## **References** 

