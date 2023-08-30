# ALX Operation #OneTaskAtATime 

## Project: C - Hello World
### Task: 5

- *Start Date:* 29-08-23
- *End Date:* 30-08-23
- *Submission Date:* 30-08-23

*Name:* Samuella Manye Aglago (Ami)

## Task Objective
By the end of this task, I should:
- Know how to use the function `printf`
- Know how to see the return value of a run program

## Task Instructions Rephrased
Write a C program using the function `printf` to print the following sentence to standard output: "with proper grammar, but the outcome is a piece of art," followed by a new line.

### Solution Explanation
- The function `printf` is used to format and print data.
- It can be used to output a string with proper grammar and format.
- The new line can be added using the escape sequence `\n`.
- The function `printf` returns a non-negative number on success and `EOF` on error.

### Solution Code
```c
#include <stdio.h>

int main(void) {
    printf("with proper grammar, but the outcome is a piece of art,\n");
    return (0);
}
```

## Personal Notes
- The function `printf` has the following signature: `int printf(const char *format, ...)`.
- It is used to format and print data.
- The return value of `printf` represents the number of characters successfully written to standard output.
