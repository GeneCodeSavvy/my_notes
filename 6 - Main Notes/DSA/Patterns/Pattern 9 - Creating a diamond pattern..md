2024-09-22 23:16

Status : #mature 

Tags : [[Given an integer 'n' recreate a specific pattern.]]

---
**Input Section**:

Star Pattern : 

``` 
for n = 5
    * 
   ***
  *****
 *******
*********
*********
 *******
  *****
   ***
    *
```

---

**Output**:

1. **Code Formatting**:
   ```javascript
   class Solution {
       pattern9(n) {
           for (let i = 0; i < 2 * n; i++) {
               const spaces = function () {
                   if (i <= n - 1) {
                       return n - 1 - i;
                   } else if (i < 2 * n) {
                       return i - n;
                   }
               };

               const stars  = function () {
                   if (i <= n - 1) {
                       return 2 * i + 1;
                   } else {
                       return 2 * ((2 * n - 1) - i) + 1;
                   }
               };
               
               for (let j = 0; j < spaces(); j++) {
                   process.stdout.write(" ");
               }
               for (let k = 0; k < stars(); k++) {
                   process.stdout.write('*');
               }
               console.log();
           }
       }
   }
   ```

2. **Summary of Approach**:
   - The solution generates a diamond-like star pattern based on the input integer `n`. 
   - It uses nested loops to handle the number of spaces and stars for each line, leveraging the relationship between the current line index and the value of `n`.
   - Key techniques include dynamic calculation of spaces and stars based on the current iteration, effectively using conditions to differentiate between the upper and lower halves of the pattern.

3. **Pseudo Code**:
   ```pseudo
   Define function pattern9(n)
   Loop from 0 to 2 * n
       If index i <= n - 1
           Calculate spaces as n - 1 - i
           Calculate stars as 2 * i + 1
       Else
           Calculate spaces as i - n
           Calculate stars as 2 * ((2 * n - 1) - i) + 1
       Print spaces
       Print stars
   End loop
   ```

---

**Supporting Sections**:

1. **Time and Space Complexity Analysis**:
   - **Time Complexity**: O(n), where n is the input integer, since there are 2n lines printed, and each line involves simple calculations.
   - **Space Complexity**: O(1), as no additional data structures are used that scale with input size.

2. **Edge Cases Considered**:
   - Edge case for `n = 0` should handle no output.
   - For `n = 1`, the pattern should produce a single star.

3. **Optimization Potential**:
   - The current implementation is efficient; however, one could optimize further by storing results in an array and printing them in one go, reducing the number of `console.log` calls.

---
## **References** 

