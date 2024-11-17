# EX-NO-6-Pseudo-Random-Number
# AIM: 
Implementation of Pseudorandom Number Generation Using Standard library

# Algorithm:

1.Start the program and import the required libraries.

2.Seed the random number generator using the current time(i.e) rand(time(0));

3.Get the number of randon number to generate.

4.Pass the value for number of iterations and print the numbers.

5.End the program.

# PROGRAM :
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
    srand(time(NULL));
    printf("Pseudorandom numbers:\n");   
    for (int i = 0; i < count; i++) 
    {
        int random_number = (rand() % (max - min + 1)) + min;
        printf("%d ", random_number);
    }
    return 0;
}
```
# OUTPUT:
![image](https://github.com/user-attachments/assets/ff647742-e88f-4597-9726-6f168e8b5572)

# RESULT :
Thus the Implementation of Pseudorandom Number Generation Using Standard library was executed successfully.





