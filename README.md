# Off-by-One Error in Java Array Iteration

This repository demonstrates a common off-by-one error that occurs when iterating over arrays in Java. The error arises from an incorrect loop condition that leads to accessing an array element beyond its bounds. This results in an `ArrayIndexOutOfBoundsException`.

The `Bug.java` file contains the erroneous code, while `BugSolution.java` shows the corrected version.

## How to reproduce the error

1. Compile `Bug.java`.
2. Run the compiled code.

You should observe an `ArrayIndexOutOfBoundsException`.

## Solution

The solution involves correcting the loop condition to ensure that the loop iterates only up to (but not including) the array's length. This prevents accessing the element at index `arr.length`, which is beyond the valid range of indices.