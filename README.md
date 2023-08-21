# Calculator-in-c-programming-
This code snippet encapsulates the essence of a basic calculator through a concise and elegant implementation. The program's user-centric approach thrives in presenting users with a menu of mathematical operations, enabling them to input operands and swiftly receive accurate results.
This C program is a simple calculator that allows users to perform basic arithmetic operations. It presents users with a menu to choose from four different operations: addition, subtraction, multiplication, and division. After selecting an operation, users input two numbers on which the chosen operation will be performed. The program then uses a `switch` statement to execute the selected operation and displays the result. If the user provides an invalid choice, the program informs them by printing "Invalid Choice." This code snippet serves as a basic foundation for a calculator program, and it showcases how to take user input, perform calculations, and present results in a clear and concise manner.
_________________________________________________________________________________________________________________________________________________________________________
                                                                    MAIN CODES STARTS FROM HERE ⬇️
-------------------------------------------------------------------------------------------------------------------------------------------------------------------------
#include<conio.h>
#include<stdio.h>

int main()
{
    char Result,choice;
    int n1,n2;

    printf("Choose an operand:-\n1.Addition\n2.Subtraction\n3.Multiplication\n4.Division\n");
    scanf("%c",&choice);

    printf("ENTER A NUMBER 1 :");
    scanf("%d",&n1);
    
     printf("ENTER A NUMBER 2 :");
    scanf("%d",&n2);
   
    switch(choice)
    {
        case'1':
        printf("%d + %d = %d", n1, n2, n1 + n2);
        break;

        case'2':
        printf("%d - %d = %d", n1, n2, n1 - n2);
        break;

        case'3':
        printf("%d * %d = %d", n1, n2, n1 * n2);
        break;

        case'4':
        printf("%d / %d = %d", n1, n2, n1 / n2);
        break;


        default: 
        printf("Invalid Choice.");

    }
    return 0;


}
