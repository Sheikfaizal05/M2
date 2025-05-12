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
    int m, n;

    scanf("%d", &m);
    scanf("%d", &n);

    for (int i = m; i <= n; i++) {
        if (i % 2 == 0) {
            printf("%d ", i);
        }
    }

    return 0;
    }

## OUTPUT:
![Screenshot 2025-05-12 225347](https://github.com/user-attachments/assets/21ad0015-343e-4df9-b4d8-9d32ab7457a8)











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
    int rows;

    scanf("%d", &rows);

    for (int i = 1; i <= rows; i++) {
        for (int j = 1; j <= i; j++) {
            printf("* ");
        }
        printf("\n");
    }

    return 0;
    }


## OUTPUT:

![image](https://github.com/user-attachments/assets/136392b0-e2e4-4c04-a5c3-3a0cc048542e)




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

    void add(int num1, int num2) {
    printf("Addition: %d\n", num1 + num2);
     }

    void subtract(int num1, int num2) {
    printf("Subtraction: %d\n", num1 - num2);
    }

    int main() {
    int number1, number2;

    scanf("%d", &number1);
    scanf("%d", &number2);

    add(number1, number2);
    subtract(number1, number2);

    return 0;
    }

## OUTPUT:
![image](https://github.com/user-attachments/assets/03fbd47d-1fe0-46f9-88f8-78aa7e172857)






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
    int number, sumOfOddDigits = 0;

    scanf("%d", &number);

    for ( ; number != 0; number /= 10) {
        int digit = number % 10;
        if (digit % 2 != 0) {
            sumOfOddDigits += digit;
        }
    }

    printf("Sum of odd digits: %d\n", sumOfOddDigits);

    return 0;
    }

## OUTPUT:
![image](https://github.com/user-attachments/assets/ba326a4e-b487-4ef9-bd7e-fcc5da974445)




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
```
#include <stdio.h>

void fact() {
    int N, fact = 1;

    scanf("%d", &N);

    for (int i = 1; i <= N; i++) {
        fact *= i;
    }

    printf("Factorial: %d\n", fact);
}

int main() {
    fact();
    return 0;
}
```
## OUTPUT:
![image](https://github.com/user-attachments/assets/2bb1b94d-77e4-4d47-8db5-b9f2583ccff0)

## RESULT:
The program correctly computes the factorial of a given number using a separate function and displays the result.
 
