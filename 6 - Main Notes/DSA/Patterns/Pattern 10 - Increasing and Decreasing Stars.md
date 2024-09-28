2024-09-23 01:34

Status : #mature 

Tags : [[Given an integer 'n' recreate a specific pattern.]]

---
## Code (JavaScript)

```javascript
class Solution {
    pattern10(n) {
        let str = ''
        for (let i = 0; i < (2 * n - 1); i++) {
            if (i < n) {
                str += '*'
            } else {
                str = str.slice(0,-1)
            }
            console.log(str)
        }
    }
}
```

## Summary of Approach

This solution uses a single loop to generate a pattern of increasing and then decreasing stars. It builds a string by adding stars for the first half of iterations, then removes stars for the second half. The pattern is printed line by line using `console.log()`, creating a visual representation of increasing and decreasing stars.

## Pseudo Code

```pseudo
Initialize an empty string
Loop from 0 to (2 * n - 1):
    If current iteration < n:
        Add a star to the string
    Else:
        Remove the last star from the string
    Print the current string
```

## Time and Space Complexity Analysis

- Time Complexity: O(n), where n is the input number. The loop runs for 2n-1 iterations.
- Space Complexity: O(n), as the maximum length of the string is n characters.

## Edge Cases Considered

- The solution handles the case when n = 1, printing a single star.
- It correctly handles all positive integer inputs for n.

## Optimisation Potential

The current solution is already optimised for time complexity. However, to optimize for space, we could avoid storing the entire string and instead print the required number of stars directly in each iteration.

## Visualisation Aid

Here's a visual representation of how the pattern evolves for n = 5:

```
*
**
***
****
*****
****
***
**
*
```

Each line represents one iteration of the loop, showing how stars are added and then removed to create the pattern.


---
## **References** 

