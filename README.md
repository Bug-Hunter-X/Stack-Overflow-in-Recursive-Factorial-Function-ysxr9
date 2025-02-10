# Hack Recursion Bug
This repository demonstrates a common error in recursive functions written in Hack: stack overflow. The `foo` function calculates the factorial of a number recursively. However, for large inputs, the function will exceed the maximum recursion depth, resulting in a stack overflow error.

## Bug
The `bug.hack` file contains the code with the error.  The factorial function is implemented recursively. This approach works for small inputs but will fail for larger numbers because it uses more stack space per call.

## Solution
The `bugSolution.hack` file provides a solution that uses an iterative approach to calculate the factorial. This avoids stack overflow errors, even for large input values.

## How to reproduce the bug
1. Clone this repository.
2. Compile the `bug.hack` file using the Hack compiler.
3. Run the compiled code with a large input value for `foo`, such as 1000.  You should observe a stack overflow error.

## How to solve the bug
1. Refer to the code in the `bugSolution.hack` file. This example uses an iterative approach that avoids the stack overflow issue.
2. Compile and run the `bugSolution.hack` file. It should correctly calculate the factorial of larger numbers without encountering errors.