# Additional Test Cases

Run each test independently, starting with `top = -1`.

## Test case 1 — Pop from an empty Stack

Operations:
```c
display();
item = pop();
printf("Popped: %d\\n", item);
```

Expected behavior:
- Prints `Stack is Empty`.
- Prints `Stack Underflow`.
- `pop()` returns `-1`.
- `top` remains `-1`.

## Test case 2 — Fill the Stack to capacity

Operations:
```c
push(1);
push(2);
push(3);
push(4);
push(5);
display();
```

Expected behavior:
- All five pushes succeed.
- Displayed Stack: `1 2 3 4 5`.
- `top` is `4`.

## Test case 3 — Overflow, then pop

Operations:
```c
push(1);
push(2);
push(3);
push(4);
push(5);
push(6);
item = pop();
printf("Popped: %d\\n", item);
display();
```

Expected behavior:
- `push(6)` prints `Stack Overflow`.
- `pop()` returns `5`.
- Displayed Stack: `1 2 3 4`.
- `top` is `3`.

Record the actual compiler output for each test in the assignment report.
