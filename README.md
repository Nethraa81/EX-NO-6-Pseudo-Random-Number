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

int main() 
{
    int count, min, max;

    printf("Enter the number of random numbers to generate: ");
    scanf("%d", &count);

    printf("Enter the minimum value: ");
    scanf("%d", &min);

    printf("Enter the maximum value: ");
    scanf("%d", &max);

    if (min > max) {
        printf("Error: Minimum value cannot be greater than maximum value.\n");
        return 1;
    }

    srand(time(NULL));  // Seed the random number generator

    printf("Pseudorandom numbers:\n");
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d\n", random_number);
    }

    return 0;
}

```

# OUTPUT:

<img width="682" height="432" alt="image" src="https://github.com/user-attachments/assets/24241797-f0a5-4c06-af0c-3b2ffb3b9757" />


# RESULT:

Thus the execution of the Pseudorandom Number Generation Using Standard library has executed successfully.
