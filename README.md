**Introduction**:

This documentation elucidates the task accomplished during the Codtech IT Solutions Internship program assigned to Aparna Singh Rajawat, with ID COD5739. The task entails developing a Java program for a simple calculator with advanced features, including addition, subtraction, multiplication, division, exponentiation, and the option to quit.

**Task Description**:
Aparna Singh Rajawat's assignment during the Codtech IT Solutions Internship program was to create a Java program for a simple calculator. The calculator is expected to offer basic arithmetic operations and advanced functionalities such as exponentiation. Additionally, the program should allow users to exit at their discretion.

Intern Information: 
Name: Aparna Singh Rajawat
Intern ID: COD5739

**Implementation**:
The implementation of the task involves utilizing Java programming language to create a simple yet efficient calculator program. The code employs a 'while' loop for functionality efficiency. Below is the code implementation.

import java.util.Scanner;

public class SimpleCalculator {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        int operator, n1, n2;
      
        while (true) {
            System.out.println("1 - Add \n2 - Subtract\n3 - Multiply\n4 - Divide \n5 - Exponentiation \n6 - Quit");
            System.out.print("Choose operator: ");
            operator = sc.nextInt();

            if (operator == 6) {
                System.out.println("Calculator is exiting. Goodbye!");
                break;
            }

            System.out.print("Enter first number: ");
            n1 = sc.nextInt();
            System.out.print("Enter second number: ");
            n2 = sc.nextInt();
            int result = 0; 

            switch (operator) {
                case 1:
                    result = n1 + n2;
                    break;  
                case 2:
                    result = n1 - n2;
                    break;  
                case 3:
                    result = n1 * n2;
                    break;  
                case 4:
                    result = n1 / n2;
                    break;  
                case 5:
                    result = (int) Math.pow(n1, n2);
                    break;
                default:
                    System.out.println("Invalid choice. Please choose again.");
                    System.out.println("Entered operator is not valid.");
            }
            System.out.println("Result is " + result);
        }  
        sc.close();
    }
}

**Features**:

. Menu-Driven Interface
. Arithmetic Operations
. Error Handling
. Looping Structure
. Resource Management
**Code Explanation** :
The program initiates by initializing a Scanner object to read user input. It then enters a while loop to continuously prompt the user for input until they opt to quit by entering '6'. Within each iteration of the loop, the menu of operation choices is displayed, and the user selects an operation. If the user chooses to quit, the program exits the loop and displays a farewell message. Otherwise, the program prompts the user to input two numbers for the selected operation. Based on the chosen operator, the program performs the corresponding arithmetic operation and displays the result. After the loop ends, the Scanner object is closed to release system resources.

**Execution Example**:

1 - Add 
2 - Subtract
3 - Multiply
4 - Divide 
5 - Exponentiation 
6 - Quit
Choose operator: 1
Enter first number: 5
Enter second number: 3
Result is 8

1 - Add 
2 - Subtract
3 - Multiply
4 - Divide 
5 - Exponentiation 
6 - Quit
Choose operator: 4
Enter first number: 10
Enter second number: 2
Result is 5

1 - Add 
2 - Subtract
3 - Multiply
4 - Divide 
5 - Exponentiation 
6 - Quit
Choose operator: 7
Invalid choice. Please choose again.
Entered operator is not valid.

1 - Add 
2 - Subtract
3 - Multiply
4 - Divide 
5 - Exponentiation 
6 - Quit
Choose operator: 6
++++Calculator is exiting. Goodbye!++++
**User Interaction**:

The user is presented with a menu of operation choices.
They select an operation by entering the corresponding number.
They input two numbers for the selected operation.
The result of the operation is displayed.
They can choose to perform another calculation or exit the program.

**Conclusion**:
The Simple Calculator program provides a straightforward solution for basic arithmetic calculations. Its user-friendly interface, error handling, and resource management enhance its usability and effectiveness. The modular structure of the code ensures scalability and maintainability.
