1. `final result:  20` is printed.
2. `final result:  undefined` is printed.
3. `final result:  20` is printed.
4. It throws a `ReferenceError: result is not defined`. Because `result` is defined only in the `if` block, we will not be able to access it in the `else` block, so we receive an error.
5. It throws a `TypeError: Assignment to constant variable.` because we are trying to reassign `result` at `result = num1 + num2` despite `result` being a `const` variable.
6. It throws a `ReferenceError: result is not defined` because `result` is defined only in the `if` block but we are trying to access it in the `else` block.