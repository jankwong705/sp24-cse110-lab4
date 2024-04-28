1. `3` is printed. After the loop, `i` will become `3`. Because `i` is a `var` variable, it can be accessed throughout the whole function block. Hence, we can print it outside of the loop block.
2. `150` is printed. After the loop, `discountedPrice` will become `150`. Because `discountedPrice` is a `var` variable, it can be accessed throughout the whole function block. Hence, we can print it outside of the loop block.
3. `150` is printed. Because `finalPrice` is a `var` variable, it can be accessed throughout the function block, so it can also be changed within the loop. After the loop, `finalPrice` will become `150`. Because `finalPrice` is a `var` variable, it can be accessed throughout the whole function block. Hence, we can print it outside of the loop block after we changed it inside the loop block.
4. `[ 50, 100, 150 ]` is returned. Because `discounted` is a `var` variable, it can be accessed throughout the function block, so it can have elements added to it within the loop. After the loop, `discounted` will become `[ 50, 100, 150 ]`. Because `finalPrice` is a `var` variable, it can be accessed throughout the whole function block. Hence, we can return it after it has been modified inside the loop.
5. It throws `ReferenceError: i is not defined`. Because `i` is a `let` variable, it can only be accessed within the loop block. As we tried to access it outside of the loop block, we will receive an error.
6. It throws `ReferenceError: discountedPrice is not defined`. Because `discountedPrice` is a `let` variable, it can only be accessed within the loop block. As we tried to access it outside of the loop block, we will receive an error.
7. `150` is printed. `finalPrice` is a `let` variable inside the whole function block, which means we can reassign or access it anywhere in the function block. Because the loop block is within the function block, we can reassign `finalPrice` inside it. As we exits the loop block, we are still in the function block, so `150` will be printed.
8. `[ 50, 100, 150 ]` is returned. `discounted` is a `let` variable inside the whole function block, which means we can reassign or access it anywhere in the function block. Because the loop block is within the function block, we can add elements to `discounted` inside it. As we exits the loop block, we are still in the function block, so `[ 50, 100, 150 ]` will be returned.
9. It throws `ReferenceError: i is not defined`. Because `i` is a `let` variable inside the loop block, if we try to access it outside of the loop block, it is not allowed.
10. `3` is printed. Because `length` is a `const` variable, it can be accessed within the block it is defined in (just like a `let` variable). Because the loop block is within the function block, we can access `length` inside it. As we exit the loop block, we are still in the function block, so we can print it. Because we didn't reassign it, no errors are thrown.
11. `[ 50, 100, 150 ]` is returned. Because `discounted` is a `const` variable, it can be accessed within the block it is defined in (just like a `let` variable). Because the loop block is within the function block, we can access `discounted` inside it. Because we didn't reassign `discounted` (we are just adding elements to it), no errors are thrown. As we exit the loop block, we are still within the function block, so we can return it.
12. 
    A. `student.name`

    B. `student['Grad Year]`

    C. `student.greeting()`

    D. `student['Favorite Teacher].name`

    E. `student.courseLoad[0]`
13. 
    A. The output is `'32'` because `2` maps to the string `'2'`.

    B. The output is `1` because `'3'` maps to `3`.

    C. The output is `3` because `null` maps to `0`.

    D. The output is `'3null'` because `null` maps to `'null'`.

    E. The output is `4` because `true` maps to `1`.

    F. The output is `0` because `false` and `null` both map to `0`.

    G. The output is `'3undefined'` because `undefined` maps to `'undefined'`.

    H. The output is `Nan` because `undefined` gets converted to `NaN`. 
14. 
    A. The output is `true` because `'2'` gets converted to `2`.

    B. The output is `false` because both `'2'` and `'12'` are strings, and `'2'` is lexicographically after `'12'`.

    C. The output is `true` because `'2'` gets converted to `2`.

    D. The output is `false` because we are doing a strict equality check without type conversions, so `'2'` won't be converted to `2`.

    E. The output is `false` because `true` maps to `1` and `1` is not equal to `2`.

    F. The output is `true` because `Boolean(2)` is `true`.

15. The regular equality `==` will convert variables to different types as necessarily, but the strict equality `===` will do comparisons without type conversions. 
16. (in `part2-question16.js`)
17. The result would be `[ 2, 4, 6 ]`. We first pass `[1, 2, 3]` and the `doSomething` function into the `modifyArray` function. Within the loop in `modifyArray`, `doSomething` is going to be called on each element of `[1, 2, 3]`, appending the modified elements to `newArr`, which would be returned at the end. Therefore, the result is `[ 2, 4, 6 ]`.
18. (in `part2-question18.js`)
19. The output is `1 4 3 2`. The program prints out `1 4 3` immediately and prints out `2` after a second.