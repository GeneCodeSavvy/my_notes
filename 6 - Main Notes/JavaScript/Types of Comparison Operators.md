2024-08-27 14:57

Status : #baby 

Tags : [[Operators]]

A comparison operator compares its operands and returns a logical value based on whether the comparison is true.
In most cases, if the two operands are not of the same type, JavaScript attempts to convert them to an appropriate type for the comparison. The sole exceptions to type conversion within comparisons involve the `===` and `!==` operators, which perform strict equality and inequality comparisons.

Examples of use below with reference to sample code. 

```js
const var1 = 3;
const var2 = 4;
```


| Sr. No. | Operator                     | Description                                                                      | Examples returning *true*   |
| ------- | ---------------------------- | -------------------------------------------------------------------------------- | --------------------------- |
| 1.      | Equal ( == )                 | Returns `true` if operands are equal.                                            | `3 == var1`, `"3" == var1`  |
| 2.      | Not Equal ( != )             | Returns `true` if operands are not equal.                                        | `var1 != 4`, `var2 != '3'`  |
| 3.      | Strict Equal ( !== )         | Returns `true` if operands are equal and of same type.                           | `3 === var1`                |
| 4.      | Greater than ( > )           | Returns `true` if the left operand is greater than the right operand.            | `var2 > var1`, `"12" > 2`   |
| 5.      | Greater than or equal ( >= ) | Returns `true` if the left operand is greater than or equal to the right operand | `var2 >= var1`, `var1 >= 3` |
| 6.      | Less than ( < )              | Returns `true` if the left operand if smaller than the right operand             | `var1 < var2`, `"2" < 12`   |
| 7.      | Less than equal to ( <= )    | Returns `true` if the left operand is smaller than or equal to the right operand | `var1 <= var2`, `var2 <= 5` |

## **References** 
1. MDN docs.