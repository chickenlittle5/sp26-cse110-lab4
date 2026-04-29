1. This would print 3. Since `i = 2` is the last number inside the loop, the `i++` increments `i` and since it's `var`, then it would print 3. 
2. This would print 150 because the last element in the array is 300 and when you discount that by 50%, it would be 150
3. This would print 150  because `finalPrice` is declared using `var`, which gives it function scope, making it accessible outside the loop.
4. The function returns `[50, 100, 150]` because for each price in the array, the function calculates the discounted price by multiplying by `(1 - discount)` and rounds it to two decimal places. Each result is pushed into the `discounted` array, which is returned at the end.
5. Line 12 will cause a `ReferenceError` because `i` is declared using `let` inside the `for` loop, making it block-scoped and not accessible outside the loop.
6. Line 13 will cause a `ReferenceError` because `discountedPrice` is declared using `let` inside the loop and is not accessible outside of that block.
7. Line 14 will print `150` because `finalPrice` is declared with `let` in the function scope (outside the loop) and retains the last value assigned during the final iteration.
8. The function returns `[50, 100, 150]` because for each price in the array, the function calculates the discounted price by multiplying by `(1 - discount)` and rounds it to two decimal places. Each result is pushed into the `discounted` array, which is returned at the end.
9. Line 11 will cause a `ReferenceError` because `i` is declared using `let` inside the `for` loop, making it block-scoped and not accessible outside the loop.
10. Line 12 will print `3` because `length` is declared using `const` in the function scope, so it is accessible outside the loop and holds the value `prices.length`, which is 3.

11. The function returns `[50, 100, 150]` because for each price in the array, the function calculates the discounted price by multiplying by `(1 - discount)` and pushes each result into the `discounted` array, which is returned at the end.

12. Notation
    1.  `student.name`
    2.  `student['Grad Year']`
    3.  `student.greeting()`
    4.  `student['Favorite Teacher'].name`
    5.  `student.courseLoad[0]`
13. Arithmetic
    1. `'3' + 2` = `'32'` because `+` with a string performs concatenation.
    2. `'3' - 2` = `1` because `-` forces numeric conversion (`'3'` becomes 3).
    3. `3 + null` = `3` because `null` is coerced to 0.
    4. `'3' + null` = `'3null'` because `+` with a string concatenates.
    5. `true + 3` = `4` because `true` is coerced to 1.
    6. `false + null` = `0` because `false` becomes 0 and `null` becomes 0.
    7. `'3' + undefined` = `'3undefined'` because of string concatenation.
    8. `'3' - undefined` = `NaN` because `undefined` cannot be converted to a number.
14. Comparison
    1. `'2' > 1` = `true` because `'2'` is coerced to the number 2.
    2. `'2' < '12'` = `false` because strings are compared lexicographically.
    3. `2 == '2'` = `true` because `==` performs type coercion.
    4. `2 === '2'` = `false` because the types are different.
    5. `true == 2` = `false` because `true` becomes 1 and 1 is not equal to 2.
    6. `true === Boolean(2)` = `true` because `Boolean(2)` evaluates to `true` and the types match.
15. Difference between `==` and `===`. `==` checks for equality after performing type coercion, meaning it converts values to the same type before comparing.  `===` checks for strict equality and does not perform type coercion, so both value and type must be the same.
16. see `part2-question16.js`.
17. The result is `[2, 4, 6]` because `modifyArray` loops through `[1, 2, 3]` and applies the callback function `doSomething` to each element. Since `doSomething` returns `num * 2`, the values become `1 * 2 = 2`, `2 * 2 = 4`, and `3 * 2 = 6`. Each result is pushed into `newArr`, which is returned at the end.
18. see `part2-question18.js`. 
19. The output is `1 4 3 2` because `console.log(1)` runs first synchronously, followed by `console.log(4)`. The `setTimeout` with 0 ms delay prints `3` after the current call stack is empty, and the `setTimeout` with 1000 ms delay prints `2` last after one second.
