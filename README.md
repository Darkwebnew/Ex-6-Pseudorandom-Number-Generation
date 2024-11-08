# Ex-6 PSEDUDORANDOM NUMBER GENERATION

<br>

## DATE:

<br>

## AIM:

<br>

To implement Pseudorandom Number Generation using the standard library functions in C.

<br>

## ALGORITHM:

<br>

Step 1: Seed the random number generator using srand() to initialize it with a starting value.

<br>

Step 2: Generate pseudorandom numbers using rand().

<br>

Step 3: To ensure different results on each execution, seed srand() with a dynamic value like the current time (time(NULL)).

<br>

Step 4: Use modulo operation to limit the range of generated numbers.

<br>

## PROGRAM:

<br>

```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main() {
    // Seed the random number generator with the current time
    srand(time(0));

    // Generate and print 5 pseudorandom numbers in the range [0, 99]
    printf("Pseudorandom numbers:\n");
    for (int i = 0; i < 5; i++) {
        int random_number = rand() % 100;  // Limit range to 0-99
        printf("%d ", random_number);
    }
    printf("\n");

    return 0;
}
```

<br>

## OUTPUT:

<br>

![image](https://github.com/user-attachments/assets/d6334ea1-13df-47e6-80c5-1510e3c18bfd)

<br>

## RESULT:

<br>

Thus, the pseudorandom number generation was successfully implemented using the standard library functions srand() and rand().
