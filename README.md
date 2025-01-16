# Julia Function Bug

This repository demonstrates a subtle bug in a Julia function that arises when handling negative inputs.

The function `myfunction` is intended to square the input, returning a positive number regardless of input sign. However, due to the use of the `^` operator, it produces incorrect results for negative numbers.

The `bug.jl` file contains the buggy code, and `bugSolution.jl` provides a corrected version using the `^2` operator which always returns a non-negative number.  The difference in behavior is explained in the comments.

This demonstrates the importance of understanding operator precedence and the subtle differences between mathematical operators in Julia and their expected behavior.