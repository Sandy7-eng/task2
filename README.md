# Stack Operations Using an Array (C)

This repository contains the C program for the **Code Trace Challenge – Think, Trace, Predict and Verify** assignment.

## Files

- `stack_array.c` — Original Stack implementation and operation sequence.
- `expected_output.txt` — Output predicted from the manual trace.
- `test_cases.md` — Three additional test cases and their expected results.

## Concepts demonstrated

- Stack implementation using an array
- LIFO (Last In, First Out)
- `push()`, `pop()`, and `display()` operations
- Stack overflow and underflow
- Tracking the `top` index

## Compile and run

Using GCC:

```bash
gcc stack_array.c -o stack_array
./stack_array
```

On Windows with MinGW:

```bash
gcc stack_array.c -o stack_array.exe
stack_array.exe
```

## Expected behavior

The array has a capacity of five elements. The attempt to push `70` occurs while the Stack is full, so it prints `Stack Overflow`. After all valid elements are popped, one more `pop()` prints `Stack Underflow` and returns `-1`.

The final logical Stack is empty and `top` is `-1`.

## Notes

The program is preserved in its original form for assignment tracing. Its `pop()` function uses `-1` as an error sentinel; this can be ambiguous if `-1` is also a valid data element. A status-returning version can avoid that limitation.
