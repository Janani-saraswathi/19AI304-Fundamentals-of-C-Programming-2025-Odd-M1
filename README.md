# IAPR-1- Module 1 - FoC
## 1. Implementation of basic C programs using Literals,Consonants, Variables, Data types.
## 2. Implementation of different categories of operators.
# Ex.No:1
  Build a C program to demonstrate the usage of different types of literals: integer, float, character, and string.  
# Date : 24.12.25
# Aim:
To build a C program that prints integer, float,character, and string literals on the console using the printf() function.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside the main() function, use printf() to display each literal along with its size in bytes using sizeof() :
  
   3.1 Integer literal (e.g., 10) using `%d`
   
   3.2 Float literal (e.g., 3.14) using `%f`
   
   3.3 Character literal (e.g., 'A') using `%c`
   
   3.4 String literal (e.g., "Hello C") using `%s`
   
### Step 4: 
   Stop
# Program:
```
#include <stdio.h>

int main() {
    // Integer literals
    int a = 10;
    int b = 075;      // Octal literal
    int c = 0x2A;     // Hexadecimal literal

    // Floating-point literals
    float x = 3.14f;
    double y = 2.5e3; // Scientific notation

    // Character literals
    char ch1 = 'A';
    char ch2 = '\n';  // Escape character

    // String literal
    char str[] = "Hello, C Programming!";

    // Output
    printf("Integer Literals:\n");
    printf("a = %d\nb = %d\nc = %d\n\n", a, b, c);

    printf("Floating-point Literals:\n");
    printf("x = %.2f\ny = %.2lf\n\n", x, y);

    printf("Character Literals:\n");
    printf("ch1 = %c\n", ch1);
    printf("ch2 is a newline character\n\n");

    printf("String Literal:\n");
    printf("%s\n", str);

    return 0;
}
```
# Output:
<img width="1920" height="1018" alt="c1" src="https://github.com/user-attachments/assets/d9451cee-6785-45ce-b769-f858e0a5950f" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:2
  Build a C program to display the value of a macro constant and a constant variable.
# Date : 24.12.25
# Aim:
  To build a C program that demonstrates the use of macro constants and constant variables.
# Algorithm:
### Step 1:
  Start  
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Define a macro constant `PI` with value `3.14159` using `#define`.
### Step 4: 
   Inside `main()`:
   
   4.1 Declare a constant integer variable `DAYS`
   
   4.2 Initialize it with the value `7`
   
### Step 5:  
  Use `printf()` to display the values of `PI` and `DAYS`.     
### Step 6:  
  Stop
# Program:
```
#include <stdio.h>

// Macro constant
#define PI 3.14

int main() {
    // Constant variable
    const int MAX = 100;

    printf("Macro constant PI = %.2f\n", PI);
    printf("Constant variable MAX = %d\n", MAX);

    return 0;
}
```
# Output:
<img width="1920" height="1080" alt="c2" src="https://github.com/user-attachments/assets/45cb171e-6a5b-4480-9ba8-94e5d53961af" />


# Result: 

Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:3
  Build a C program to demonstrate the use of different data types such as int, float, double, and char, and display their values using printf().
# Date : 24.12.25
# Aim:
  To build a C program that declares variables of various data types—integer, float, double, and character—initializes them, and prints their values on the screen.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Inside main(), declare and initialize variables of types int, float, double, and char.
### Step 4: 
   Display their values using printf().
### Step 5:    
   Stop
# Program:
```
#include <stdio.h>

int main() {
    int i = 25;
    float f = 12.5f;
    double d = 123.456789;
    char c = 'A';

    printf("Integer value: %d\n", i);
    printf("Float value: %.2f\n", f);
    printf("Double value: %.6lf\n", d);
    printf("Character value: %c\n", c);

    return 0;
}
```
# Output:
<img width="1920" height="1080" alt="c3" src="https://github.com/user-attachments/assets/c750f4f7-9c30-4848-81fe-0cf1091880a9" />

# Result: 

# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:4
  Build a C program to perform arithmetic and bitwise operations on two integers entered by the user. The program should display: Arithmetic operations: addition, subtraction, multiplication, division, and remainder. Bitwise operations: AND, OR, XOR, left shift, right shift, and NOT.
# Date : 24.12.25
# Aim:
  To build a C program that takes two integers as input and demonstrates the arithmetic and bitwise operations, displaying the results of each operation.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Declare two integer variables a and b.
### Step 4: 
   Prompt the user to enter two integers and read the input using scanf().
### Step 5:    
   Perform arithmetic operations on a and b:
   #### Sum (a + b)
   #### Difference (a - b)
   #### Product (a * b)
   #### Quotient (a / b)
   #### Remainder (a % b)
### Step 6: 
  Perform bitwise operations on a and b:
  #### AND (a &amp; b)
  #### OR (a | b)
  #### XOR (a ^ b)
  #### Left shift (a << b)
  #### Right shift (a >> b)
  #### Bitwise NOT of a (~a) and b (~b)
### Step 7:   
  Display the results of all operations using printf().
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>

int main() {
    int a, b;

    // Input two integers
    printf("Enter two integers: ");
    scanf("%d %d", &a, &b);

    // Arithmetic operations
    printf("\nArithmetic Operations:\n");
    printf("Addition: %d\n", a + b);
    printf("Subtraction: %d\n", a - b);
    printf("Multiplication: %d\n", a * b);

    if (b != 0) {
        printf("Division: %d\n", a / b);
        printf("Remainder: %d\n", a % b);
    } else {
        printf("Division and Remainder: Not possible (division by zero)\n");
    }

    // Bitwise operations
    printf("\nBitwise Operations:\n");
    printf("AND (a & b): %d\n", a & b);
    printf("OR  (a | b): %d\n", a | b);
    printf("XOR (a ^ b): %d\n", a ^ b);
    printf("Left Shift (a << 1): %d\n", a << 1);
    printf("Right Shift (a >> 1): %d\n", a >> 1);
    printf("NOT (~a): %d\n", ~a);

    return 0;
}
```
# Output:
<img width="1920" height="1080" alt="c4" src="https://github.com/user-attachments/assets/39d46a4b-d4a7-47ba-a7b8-9ecfe5fca8b8" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


# 19AI304-Fundamentals-of-C-Programming-2025-Odd
# IAPR-1- Module 1 - FoC
# Ex.No:5
  Develop a C program to check whether a given character is a vowel, consonant, digit, or special symbol using the ternary operator.
# Date : 24.12.25
# Aim:
  To develop and implement a C program that classifies a character as a vowel, consonant, digit, or special symbol using the ternary operator.
# Algorithm:
### Step 1:
  Start
### Step 2: 
  Include the standard input-output library: #include<stdio.h>.
### Step 3: 
  Input a character ch from the user.
### Step 4: 
   Check if ch is a digit ('0' to '9').
   
   If true → Print "Digit" → Go to Step 8.
   
   If false → Go to Step 5.
   
### Step 5:    
   Check if ch is an alphabet letter ('A' - 'Z' or 'a' – 'z').
   
   If true → Go to Step 6.
   
   If false → Go to Step 7.
   
### Step 6: 
   Check if ch is a vowel (a, e, i, o, u or A, E, I, O, U).
   
   If true → Print "Vowel" → Go to Step 8.
   
   If false → Print "Consonant" → Go to Step 8.
   
### Step 7:   
   Print "Special Symbol".
### Step 8:   
  Stop
# Program:
```
#include <stdio.h>

int main() {
    char ch;

    printf("Enter a character: ");
    scanf("%c", &ch);

    (ch >= '0' && ch <= '9') ?
        printf("'%c' is a Digit\n", ch) :
    ((ch >= 'A' && ch <= 'Z') || (ch >= 'a' && ch <= 'z')) ?
        ((ch == 'A' || ch == 'E' || ch == 'I' || ch == 'O' || ch == 'U' ||
          ch == 'a' || ch == 'e' || ch == 'i' || ch == 'o' || ch == 'u') ?
            printf("'%c' is a Vowel\n", ch) :
            printf("'%c' is a Consonant\n", ch)) :
        printf("'%c' is a Special Symbol\n", ch);

    return 0;
}
```
# Output:
<img width="1920" height="1080" alt="c5" src="https://github.com/user-attachments/assets/0457f7c0-3cfd-4109-9923-6c208ca34305" />

# Result: 
Thus, the program was implemented and executed successfully, and the required output was obtained.


