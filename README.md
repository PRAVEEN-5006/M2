# EX-06 - Looping
## AIM:
Write a C program to print even numbers ranging from M to N (including M and N values).

## ALGORITHM:
1.	Declare two integer variables to store the values of M and N.
2.	Use the printf function to prompt the user to enter the values of M and N.
3.	Use the scanf function to read the values of M and N from the user.
4.	Use a loop (for or while) to iterate from M to N.
5.	Inside the loop, check if the current number is even.
6.	If the current number is even, print it.
7.	Continue the loop until you have iterated through all numbers from M to N.

## PROGRAM:
#include <stdio.h>

int main() {
    int M, N; 
    printf("Enter the value of M: ");
    scanf("%d", &M);

    printf("Enter the value of N: ");
    scanf("%d", &N);
    printf("Even numbers from %d to %d are:\n", M, N);
    for (int i = M; i <= N; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }

    printf("\n"); 

    return 0; 
}

## OUTPUT:
![Screenshot 2025-04-28 135141](https://github.com/user-attachments/assets/d49664ae-e858-4c6b-9b32-0263a62e5e83)











## RESULT:
Thus the program to print even numbers ranging from M to N (including M and N values) has been executed successfully
 
 


# EX-07-Nested-loop

## AIM:

Write a C program to print the given triangular pattern using loop.

## ALGORITHM:

1.	Declare a variable to store the number of rows in the triangle.
2.	Use the printf function to prompt the user to enter the number of rows.
3.	Use a loop (for or while) to iterate through each row.
4.	Inside the loop, use another loop to print the desired number of asterisks for each row.
5.	Continue the loop until you have printed the entire triangular pattern.

## PROGRAM:
#include <stdio.h>

int main() {
    int rows, i, j; 
    printf("Enter the number of rows: ");
    scanf("%d", &rows);

    for (i = 1; i <= rows; i++) {
        for (j = 1; j <= i; j++) {
            printf("* ");
        }
        printf("\n"); 
    }

    return 0; 
}


## OUTPUT:
![Screenshot 2025-04-28 135346](https://github.com/user-attachments/assets/0ddc9f41-44a9-41d4-a775-a276adf8cf89)





## RESULT:

Thus the program to print the given triangular pattern using loop has been executed successfully
 
 


# EX-08-Functions

## AIM:

Write a C program to perform addition and subtraction of two numbers using functions (with argument and without return type).

## ALGORITHM:

1.	Declare two functions, one for addition and one for subtraction. Both functions should take two integer arguments.
2.	Inside the addition & subtraction function, add & subtract the two numbers and print the result.
3.	In the main function, declare two integer variables and read their values from the user.
4.	Call the addition and subtraction functions, passing the two numbers as arguments.

## PROGRAM:
#include <stdio.h>
void add(int a, int b);
void subtract(int a, int b);

int main() {
    int num1, num2; 
    printf("Enter first number: ");
    scanf("%d", &num1);

    printf("Enter second number: ");
    scanf("%d", &num2);

    add(num1, num2);
    subtract(num1, num2);

    return 0;
}

void add(int a, int b) {
    int result = a + b;
    printf("Addition of %d and %d is: %d\n", a, b, result);
}
void subtract(int a, int b) {
    int result = a - b;
    printf("Subtraction of %d and %d is: %d\n", a, b, result);
}


## OUTPUT:
![Screenshot 2025-04-28 135528](https://github.com/user-attachments/assets/1ed45a2a-8b7b-484c-8253-eb8c371a7687)







## RESULT:

Thus the program to perform addition and subtraction of two numbers using functions has been executed successfully
 
 


# EX-09-Use For Loop

## AIM:

Write a c program to find the sum of odd digits using for loop

## ALGORITHM:

1.	Declare variables to store the input number and the sum of odd digits.
2.	Initialize the sum of odd digits to 0.
3.	Use a for loop to iterate through each digit of the input number.
4.	Inside the loop, extract the rightmost digit of the number (using the modulo operator % and division by 10).
5.	If the digit is odd, add it to the sum of odd digits.
6.	Print the sum of odd digits.

## PROGRAM:
#include <stdio.h>

int main() {
    int num, digit, sum = 0;
    printf("Enter a number: ");
    scanf("%d", &num);12345
    for (; num != 0; num = num / 10) {
        digit = num % 10; 
        if (digit % 2 != 0) { 
            sum = sum + digit;
        }
    }
    printf("Sum of odd digits = %d\n", sum);

    return 0;
}


## OUTPUT:

![Screenshot 2025-04-28 135712](https://github.com/user-attachments/assets/9bd818a6-ec41-40d3-b63c-59154318c1aa)



## RESULT:

Thus the program to find the sum of odd digits using for loop has been executed successfully.




# EX – 10 - Factorial of a Number Using a Function
## AIM:
To write a C program that calculates the factorial of a given number using a user-defined function.
## ALGORITHM:
1.	Start
2.	Declare the function fact().
3.	In the main() function, call the fact() function.
4.	In fact() function:
a.	Declare variables i, N, and fact (initialized to 1).
b.	Read an integer N from the user.
c.	Use a for loop from 1 to N:
i.	Multiply fact by i in each iteration.
d.	After the loop, print the factorial value.
5.	End

## PROGRAM:
#include <stdio.h>

void fact();

int main() {
    fact();
    return 0;
}

void fact() {
    int i, N;
    unsigned long long factorial = 1; 
    printf("Enter a number to find its factorial: ");
    scanf("%d", &N);

    if (N < 0) {
        printf("Factorial is not defined for negative numbers.\n");
        return;
    }

    for (i = 1; i <= N; i++) {
        factorial = factorial * i;
    }
    printf("Factorial of %d = %llu\n", N, factorial);
}


## OUTPUT:
![Screenshot 2025-04-28 140134](https://github.com/user-attachments/assets/27d8dcd5-e51b-4a35-9385-9df038b8764a)


## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
