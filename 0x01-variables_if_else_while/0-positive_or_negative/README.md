# ALX Operation #OneTaskAtATime 
## Project : C - Variables, if, else, while
### Task: 0
**Start Date:** 10-11-23
**End Date:** 10-11-23
**Submission Date:** -

**AUTHOR:** Ami

By the end of this task, I should:
- be able to know how to use if else control statement

**Task Instructions Rephrased:**
The code will produce a different value in the variable `n` each time you run the program. The code should not be modified.

The program's output should display the value of `n`, followed by one of the following statements:
- If `n` is greater than 0: "is positive."
- If `n` is 0: "is zero."
- If `n` is less than 0: "is negative."

Each statement should be followed by a new line.


**Solution of task in plain words:**
Using a control flow statement, `if-else`


**Solution to the task in code:**
[Task 0](./0-positive_or_negative.c)

NO ERRORS

**EXPLAINING THE CODES**
```c
srand(time(0));
n = rand() - RAND_MAX / 2;
```
In the provided code:

1. `srand(time(0));` seeds the random number generator with the current time, introducing variability based on the time. This step is often used to make the sequence of random numbers appear more random and less predictable.

2. `n = rand() - RAND_MAX / 2;` generates a random integer using `rand()`, which by default produces values between 0 and `RAND_MAX`. Subtracting `RAND_MAX / 2` centers the range of random values around zero, resulting in random integers that can be both positive and negative, making them symmetrically distributed around zero.

In summary, this code initializes the random number generator with a seed based on the current time and then generates a random integer that's centered around zero, with roughly equal chances of being positive or negative.

**NOTES**
### `srand()` function
The `srand` function in C (and C++) is used to seed the random number generator, which initializes it with a starting value known as the "seed." The primary purpose of srand is to provide an initial state for the random number generator so that it can generate a sequence of seemingly random numbers.


The `srand` function in C has the following signature:

```c
void srand(unsigned int seed);
```

Here's what the parameters mean:

- `seed`: An unsigned integer value that serves as the seed to initialize the random number generator. The specific value you provide for the seed will determine the initial state of the generator, and different seeds will produce different sequences of random numbers.

You typically call `srand` with a seed value before using the `rand` function to generate random numbers in your program. For example:

```c
srand(123); // Seed the random number generator with the value 123
int randomValue = rand(); // Generate a random number
```

Keep in mind that the choice of the seed value will affect the sequence of random numbers produced by the `rand` function, so different seeds will result in different sequences.

### `time()` function

The `time` function in C and C++ is a standard library function used to retrieve the current calendar time. It's often used to get the current time in seconds since a reference point (usually the Unix epoch, which is January 1, 1970).

Here's the signature of the `time` function:

```c
time_t time(time_t *t);
```

- `time_t` is a data type for representing time values.
- `t` is a pointer to a `time_t` object where the function stores the current time value, or it can be a null pointer (i.e., `NULL`) if you don't need the current time.

The `time` function returns the current time in seconds since the reference point as a `time_t` value. It's commonly used to seed the random number generator (as in `srand(time(0))`), measure program execution time, and perform various time-related tasks in C and C++ programs.

Here's an example of how you might use the `time` function:

```c
#include <stdio.h>
#include <time.h>

int main() {
    time_t current_time;
    time(&current_time);

    printf("Current time: %ld\n", current_time);

    return 0;
}
```

This program uses the `time` function to obtain the current time and then prints it to the console.


When you pass `0` as an argument to the `time` function, it means you're requesting the current time in seconds since the reference point, which is the Unix epoch (January 1, 1970).

### Random values that are symmetric around zero
The code subtracts `RAND_MAX` / 2 from rand() to center the range of random values around zero. This adjustment is often used when you want random numbers that are roughly centered around zero, making them equally likely to be positive or negative.

By default, the rand() function generates random values in the range [0, `RAND_MAX`], which are all positive. Subtracting `RAND_MAX` / 2 effectively shifts the range from [-`RAND_MAX` / 2, `RAND_MAX` / 2], centered around zero. This can be useful in applications where you need random values that are symmetric around zero.
