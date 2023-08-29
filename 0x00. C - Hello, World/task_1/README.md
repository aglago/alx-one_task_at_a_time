# 1-compiler
script that compiles a c program but not link it
- c program is stored in global variable $CFILE
- output should be named the same as name of c program from which it was compiled from

## Must knows
- Shell script: []()
- C program: [main.c](./main.c) but this file must be saved in a created global variable
- output file: [main.o](./main.o)

## Discovery
- can save ouput of compilation to the same name as script name by
```
gcc -o ${0%.c}.o main.c
```
where `main.c` is the program to be compiled
