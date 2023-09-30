# ALX Operation #OneTaskAtATime 
## Project : C - Hello World
### Task: 6
- *Start Date:* 04-09-23
- *End Date:* 29-09-23
- *Submission Date:* 29-08-23

*Name:* Samuella M. Aglago (Ami)

## Task Objectives
By the end of this task, I should
- Know how to use the sizeof operator
- Know the format specifier for representing the return of sizeof
- Know how to install a package on Linux

## Task Instructions Rephrased: 
Write a C program to display the sizes of various data types in both 64 bit and 32 bit systems. 
- Must install package libc6-dev-i386

### Solution of task in plain words:
The sizeof operator in C is used to find the number of bytes that a certain data type will reserve in memory.
printf can then be used to display this number of bytes

### Solution to the task in code:
[Task 6](./6-size.c)



## ERRORS
### Error 1:
```
| #include <bits/libc-header-start.h>
      |          ^~~~~~~~~~~~~~~~~~~~~~~~~~
compilation terminated.
```
This error was a result of not installing the libc6-dev-i386 package.
Error was solved by installing the package using sudo apt-get install libc6-dev-i386 .


## PERSONAL NOTES
Format specifier for the return of sizeof is %zu or %lu for 64 bit and %u for 32 bit.

