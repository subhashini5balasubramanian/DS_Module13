# EX3 Implementation of Tower of Hanoi
## AIM:
To write a C program to implement Tower of Hanoi

## Algorithm
1. Start the program.
2. Define the priority() function to return the priority of operators.
3. Initialize the string containing operators and operands.
4. Loop through each character in the string.
5. For each operator, call the priority() function to determine its priority.
6. Print the operator and its corresponding priority level.
7. End

## Program:
```
/*
Program to implement Tower of Hanoi
Developed by: SUBHASHINI.B
RegisterNumber: 212223040211
*/
#include<stdio.h>
void TOH(int n,char x,char y,char z)
{
     if (n > 0) {
        TOH(n - 1, x, z, y);
        printf("%c to %c\n", x, y);
        TOH(n - 1, z, y, x);
    }
}
int main()
{
   int n = 4; 
    TOH(n, 'A', 'B', 'C');
    return 0;
}
```

## Output:
![Screenshot 2025-04-29 091729](https://github.com/user-attachments/assets/28f1f80f-7fc8-4383-b6dc-72ea3807fd08)



## Result:
Thus, the C program to implement Tower of Hanoi using recursion is implemented successfully.
