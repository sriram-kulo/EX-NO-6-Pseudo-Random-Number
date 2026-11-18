# EX-NO-6-Pseudo-Random-Number

# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# ALGORITHM:
Start the program and import the required libraries.
Seed the random number generator using the current time(i.e) rand(time(0));
Get the number of randon number to generate.
Pass the value for number of iterations and print the numbers.
End the program.

# PROGRAM:
```
#include <stdio.h>
#include <stdlib.h>
#include <time.h>

int main(void)
{
    int count;

    printf("How many random numbers should be generated? ");
    if (scanf("%d", &count) != 1 || count <= 0) {
        printf("Please enter a positive integer.\n");
        return 1;
    }

    srand((unsigned int)time(NULL));

    printf("Random numbers:\n");
    for (int i = 0; i < count; i++) {
        printf("%d\n", rand());
    }

    return 0;
}
```
# OUTPUT:
<img width="405" height="270" alt="image" src="https://github.com/user-attachments/assets/fc57b2d4-f8b4-46f3-bb4c-4107560502a8" />

# RESULT:
Thus, the implementation of pseudorandom number generation using standard library was executed successfully.
