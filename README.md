# Ada Off-by-One Error Example

This repository demonstrates a common off-by-one error in Ada programming, specifically when iterating over array indices. Ada arrays are 1-based, not 0-based like in many other languages (such as C, C++, Java, Python, JavaScript, etc).  The example code attempts to access an array element outside of its valid range, leading to a runtime error.

The `bug.ada` file contains the erroneous code, and `bugSolution.ada` provides the corrected version.

## How to reproduce:

1. Compile `bug.ada` with an Ada compiler (e.g., GNAT).
2. Run the compiled program.  It will raise a `Constraint_Error`.
3. Compile and run `bugSolution.ada` to see the correct behavior.

## Lesson Learned:

Always pay close attention to the bounds of arrays in Ada. Remember that indexing begins at 1.