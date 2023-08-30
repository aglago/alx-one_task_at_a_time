# ALX Operation #OneTaskAtATime 

## Project: C - Hello World
### Task: 4

- *Start Date:* 29-08-23
- *End Date:* 30-08-23
- *Submission Date:* 30-08-23

*Name:* Samuella Manye Aglago (Ami)

## Task Objective
By the end of this task, I should:
- Know how to use the function `puts`
- Know how to print a string (sentence) including a double quote, "

## Task Instructions Rephrased
Write a C program using the function `puts` to print the following sentence to standard output: "programming is like building a multilingual puzzle" followed by a new line.

### Solution Explanation
- The sentence given to print out contains a double quote.
- The backslash `\` is a special character used to escape some characters so that the compiler does not interpret it in a computing sense but treats it like any other character to be printed out.
- The function `puts` already adds a trailing new line to standard output.

### Solution Code
- [4-puts.c](./4-puts.c)

## Personal Notes
- The function `puts` has the following signature: `int puts(const char *s);`
- The function can be called from the `stdio.h` header file.
- It is used to write a string `s` and a trailing new line to standard output.
- It returns a non-negative number on success and `EOF` on error.
- The non-negative integer represents the number of characters successfully written to standard output.
