# Answers: Datatype, Constant & Variable

## Question 1: What is Data Type? Explain with examples.

**Answer**:  
Data types in C define the type of data a variable can hold. Common data types include:
- `int`: Stores integers (e.g., `10`, `-5`).
- `float`: Stores floating-point numbers (e.g., `3.14`).
- `double`: Stores double-precision floating-point numbers.
- `char`: Stores a single character (e.g., `'A'`).

---

## Question 2: What is Variable? Explain with examples.

**Answer**:  
A variable is a named storage location in memory that can hold a value. Variables must be declared with a specific data type before use. For example:
```c
int age = 25;  // Declare and initialize
age = 30;      // Modify the value
```

---

## Question 3: What is Constant Variable? Explain with examples.

**Answer**:  
A constant variable is a value that cannot be changed during the execution of a program. It is declared using the `const` keyword. For example:
```c
const double PI = 3.14159;
```

---

## Question 4: What is the maximum range of each data type as per 16-bit compiler?

**Answer**:  
The maximum range of each data type in a 16-bit compiler is as follows:
- `int`: -32,768 to 32,767
- `unsigned int`: 0 to 65,535
- `char`: -128 to 127
- `unsigned char`: 0 to 255
- `float`: 3.4E-38 to 3.4E+38
- `double`: 1.7E-308 to 1.7E+308

---

## Question 5: What is Format Specifier? Explain use case of each format specifier.

**Answer**:  
Format specifiers are used in C to specify the type of data to be printed or read. Common format specifiers include:
- `%d`: Integer
- `%f`: Floating-point number
- `%c`: Character
- `%s`: String
- `%lf`: Double

Example:
```c
int num = 10;
printf("Number: %d", num);
```

---

## Question 6: Explain printf() and scanf() functions in detail.

**Answer**:  
- `printf()`: Used to print output to the console. Example:
  ```c
  printf("Hello, World!\n");
  ```
- `scanf()`: Used to read input from the user. Example:
  ```c
  int num;
  scanf("%d", &num);
  ```

---

## Question 7: Explain Keywords in C language.

**Answer**:  
Keywords are reserved words in C that have predefined meanings. Examples include `int`, `float`, `if`, `else`, `return`, etc. These cannot be used as variable names.

---

## Question 8: What are the basic rules for creating a Variable?

**Answer**:  
The basic rules for creating a variable in C are:
1. The name must begin with a letter or underscore (`_`).
2. The name can only contain letters, digits, and underscores.
3. Keywords cannot be used as variable names.
4. Variable names are case-sensitive.

Example:
```c
int age = 25;  // Valid
int 1age = 30; // Invalid
```

---


# Operator

## Question 1: What is Operator? Explain with its types.

**Answer**:  
Operators are symbols used to perform operations on variables and values. Types of operators include:
- Arithmetic Operators: `+`, `-`, `*`, `/`, `%`
- Relational Operators: `==`, `!=`, `>`, `<`, `>=`, `<=`
- Logical Operators: `&&`, `||`, `!`
- Bitwise Operators: `&`, `|`, `^`, `~`, `<<`, `>>`
- Assignment Operators: `=`, `+=`, `-=`, etc.

---

## Question 2: Describe Operator Precedence with example.

**Answer**:  
Operator precedence determines the order in which operators are evaluated. For example:
```c
int result = 10 + 5 * 2;  // Multiplication (*) is evaluated before addition (+)
```
The result is `20` because `5 * 2` is evaluated first.

---

## Question 3: Explain Type Casting or Type Conversion.

**Answer**:  
Type casting is the process of converting one data type to another. For example:
```c
int num = 10;
double result = (double)num / 3;  // Explicit type casting
```
Here, `num` is cast to `double` before division.

---


# Control Structure

## Question 1: Explain types of Control Structure.

**Answer**:  
Control structures determine the flow of a program. Types include:
1. Sequential: Executes statements in order.
2. Selection: Uses `if`, `if-else`, `switch`.
3. Iteration: Uses loops like `for`, `while`, `do-while`.

---

## Question 2: What is Flowchart? Explain all shapes used in Flowchart.

**Answer**:  
A flowchart is a graphical representation of a process. Common shapes include:
- Oval: Start/End
- Rectangle: Process
- Diamond: Decision
- Arrow: Flowline

---

## Question 3: Explain working of if else statement with example.

**Answer**:  
The `if-else` statement executes one block of code if a condition is true, otherwise another block. Example:
```c
if (x > 0) {
    printf("Positive");
} else {
    printf("Non-positive");
}
```

---

## Question 4: Explain working of ladder if else with example.

**Answer**:  
The ladder `if-else` checks multiple conditions. Example:
```c
if (x > 0) {
    printf("Positive");
} else if (x < 0) {
    printf("Negative");
} else {
    printf("Zero");
}
```

---

## Question 5: Explain working of nested if else with example.

**Answer**:  
Nested `if-else` statements are `if-else` inside another `if-else`. Example:
```c
if (x > 0) {
    if (x % 2 == 0) {
        printf("Positive Even");
    } else {
        printf("Positive Odd");
    }
}
```

---

## Question 6: Explain structure of ternary operator with example.

**Answer**:  
The ternary operator is a shorthand for `if-else`. Syntax:
```c
condition ? expression1 : expression2;
```
Example:
```c
int max = (a > b) ? a : b;
```

---

## Question 7: Explain structure of Switch case with example.

**Answer**:  
The `switch` statement selects one of many blocks of code to execute. Example:
```c
switch (day) {
    case 1: printf("Monday"); break;
    case 2: printf("Tuesday"); break;
    default: printf("Other day");
}
```

---


# Looping

## Question 1: What is Loop? Explain types of Loops.

**Answer**:  
A loop executes a block of code repeatedly. Types include:
1. `for` loop
2. `while` loop
3. `do-while` loop

---

## Question 2: Explain Entry-controlled loops with example.

**Answer**:  
Entry-controlled loops check the condition before execution. Example:
```c
for (int i = 0; i < 5; i++) {
    printf("%d", i);
}
```

---

## Question 3: Explain Exit-controlled loops with example.

**Answer**:  
Exit-controlled loops execute at least once. Example:
```c
do {
    printf("Hello");
} while (x > 0);
```

---

## Question 4: Explain Control Statements with example.

**Answer**:  
Control statements alter the flow of execution in a program. Examples include:
- `break`: Exits a loop or switch statement.
- `continue`: Skips the current iteration of a loop.
- `goto`: Jumps to a labeled statement.

Example:
```c
for (int i = 0; i < 5; i++) {
    if (i == 3) continue;  // Skip iteration when i is 3
    printf("%d ", i);
}
```

---

## Question 5: State difference between entry-controlled and exit-controlled loops.

**Answer**:  
- **Entry-controlled loops**: The condition is checked before the loop body executes (e.g., `for`, `while`).
- **Exit-controlled loops**: The condition is checked after the loop body executes (e.g., `do-while`).

---

## Question 6: What is Pattern? Explain types of Patterns.

**Answer**:  
Patterns are visual representations created using loops. Types include:
- **Pyramid patterns**
- **Diamond patterns**
- **Number patterns**

Example:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("* ");
    }
    printf("\n");
}
```

---


# Array

## Question 1: What is Array? Explain its types.

**Answer**:  
An array is a collection of elements of the same type stored in contiguous memory locations. Types of arrays include:
- **Single-dimensional arrays**: A list of elements. Example: `int arr[5];`
- **Multi-dimensional arrays**: Arrays of arrays. Example: `int arr[3][4];`

---

## Question 2: What is 1D array? Explain with example.

**Answer**:  
A 1D array is a linear collection of elements of the same type. Example:
```c
int arr[5] = {1, 2, 3, 4, 5};
```

---

## Question 3: What is 2D array? Explain with example.

**Answer**:  
A 2D array is a matrix of elements. Example:
```c
int matrix[2][2] = {{1, 2}, {3, 4}};
```

---

## Question 4: Explain the logic of finding sum of all diagonal elements.

**Answer**:  
To find the sum of diagonal elements:
```c
int sum = 0;
for (int i = 0; i < n; i++) {
    sum += matrix[i][i];
}
```

---

## Question 5: Explain the logic of finding sum of all anti-diagonal elements.

**Answer**:  
To find the sum of anti-diagonal elements:
```c
int sum = 0;
for (int i = 0; i < n; i++) {
    sum += matrix[i][n - i - 1];
}
```

---


# String

## Question 1: What is String? Explain with example in detail.

**Answer**:  
A string is a sequence of characters terminated by a null character (`'\0'`). It is used to store text. Example:
```c
char str[] = "Hello";
```
This declares a string `str` with the value "Hello".

---

## Question 2: What is ASCII value? List some important ASCII values.

**Answer**:  
ASCII values represent characters as integers. Examples:
- `A`: 65
- `a`: 97
- `0`: 48

---

## Question 3: What is NULL? Explain with example in detail.

**Answer**:  
`NULL` is a macro representing a null pointer. Example:
```c
int *ptr = NULL;
```

---

## Question 4: List some built-in string functions with example.

**Answer**:  
Common string functions:
- `strcpy`: Copy string.
- `strcat`: Concatenate strings.
- `strcmp`: Compare strings.

Example:
```c
char str1[10], str2[10];
strcpy(str1, "Hello");
strcat(str1, " World");
```

---

## Question 5: What is the use case of strcpy() function?

**Answer**:  
`strcpy` copies one string to another. Example:
```c
strcpy(dest, src);
```

---

## Question 6: What is the use case of strcat() function?

**Answer**:  
`strcat` appends one string to another. Example:
```c
strcat(dest, src);
```

---

## Question 7: What is the use case of strcmp() function?

**Answer**:  
`strcmp` compares two strings. Example:
```c
if (strcmp(str1, str2) == 0) {
    printf("Equal");
}
```

---

## Question 8: What is '\0' in C language? Explain its use case with example.

**Answer**:  
`\0` is the null character marking the end of a string. Example:
```c
char str[] = "Hello\0World";  // Only "Hello" is considered a string
```

---

## Question 9: How to create Array of String?

**Answer**:  
An array of strings is a 2D array of characters. Example:
```c
char names[3][10] = {"Alice", "Bob", "Charlie"};
```

---

## Question 10: Explain getch() function in detail.

**Answer**:  
`getch()` reads a character from the keyboard without echoing it. Example:
```c
char ch = getch();
```

---


# User Defined Function

## Question 1: What is Function? Explain types of it.

**Answer**:  
A function is a block of code that performs a specific task. Types of functions include:
- **Library functions**: Predefined functions in libraries (e.g., `printf`, `scanf`).
- **User-defined functions**: Functions defined by the user to perform specific tasks.

---

## Question 2: What is User Defined Function (UDF)? Explain types of it.

**Answer**:  
User-defined functions are created by the programmer. Types:
1. Functions with no arguments and no return value.
2. Functions with arguments and no return value.
3. Functions with arguments and return value.

---

## Question 3: What is Recursion? Explain working of a Recursion mechanism with example.

**Answer**:  
Recursion is a function calling itself. Example:
```c
int factorial(int n) {
    if (n == 0) return 1;
    return n * factorial(n - 1);
}
```

---

## Question 4: What is Nested Function? Explain with example.

**Answer**:  
Nested functions are functions defined inside other functions. Example:
```c
void outer() {
    void inner() {
        printf("Inner function");
    }
    inner();
}
```

---


# Pointer

## Question 1: What is Pointer? Explain its use case.

**Answer**:  
A pointer is a variable that stores the memory address of another variable. Use case:
- Dynamic memory allocation
- Arrays and strings manipulation
- Function arguments (pass by reference)

Example:
```c
int a = 10;
int *p = &a;  // Pointer p holds the address of variable a
```

---

## Question 2: Explain working of sizeof() operator.

**Answer**:  
The `sizeof` operator returns the size of a data type or variable in bytes. Example:
```c
int a;
printf("%zu", sizeof(a));  // Prints the size of integer variable a
```

---

## Question 3: What is Scale of Pointer? Explain with example.

**Answer**:  
The scale of a pointer refers to the size of the data type it points to. Example:
```c
int *p;
printf("%zu", sizeof(p));  // Scale of pointer p
```

---

## Question 4: Describe Array of Pointers with example.

**Answer**:  
An array of pointers is an array where each element is a pointer. Example:
```c
int *arr[5];  // Array of 5 integer pointers
```

---

## Question 5: What is Chain of Pointer? Describe with example.

**Answer**:  
A chain of pointers is multiple pointers pointing to each other. Example:
```c
int a = 10, b = 20;
int *p1 = &a, *p2 = &b;
int **pp = &p1;  // Pointer to pointer
```

---

## Question 6: Explain Pointer with UDF in detail.

**Answer**:  
Pointers can be used in user-defined functions to pass arguments by reference, allowing the function to modify the original variable. Example:
```c
void swap(int *x, int *y) {
    int temp = *x;
    *x = *y;
    *y = temp;
}
```

---


# Structure, Union & Enumeration

## Question 1: What is Structure? Explain with example.

**Answer**:  
A structure is a user-defined data type in C that groups related variables of different data types. Example:
```c
struct Person {
    char name[50];
    int age;
};
```

---

## Question 2: What is Union? Explain with example.

**Answer**:  
A union is a user-defined data type in C that allows storing different data types in the same memory location. Example:
```c
union Data {
    int i;
    float f;
    char str[20];
};
```

---

## Question 3: What is Enumeration? Explain with example.

**Answer**:  
Enumeration is a user-defined data type in C that consists of integral constants. Example:
```c
enum Color {red, green, blue};
```

---

## Question 4: State difference between a Structure & Union.

**Answer**:  
- **Structure**: Allocates separate memory for each member.
- **Union**: Allocates a shared memory for all members (only one member can contain a value at any time).

---

## Question 5: What is Array of objects in Structure? Describe with example.

**Answer**:  
An array of objects in a structure is an array where each element is a structure. Example:
```c
struct Person arr[10];  // Array of 10 Person structures
```

---


# File Handling

## Question 1: What is File Handling? How many modes available for opening a file and which are they?

**Answer**:  
File handling in C allows programs to create, read, write, and manipulate files. Modes available for opening a file include:
- `"r"`: Opens a file for reading. The file must exist.
- `"w"`: Opens a file for writing. Creates a new file if it doesn’t exist or truncates an existing file.
- `"a"`: Opens a file for appending. Creates a new file if it doesn’t exist.
- `"r+"`: Opens a file for both reading and writing. The file must exist.
- `"w+"`: Opens a file for both reading and writing. Creates a new file if it doesn’t exist or truncates an existing file.
- `"a+"`: Opens a file for both reading and appending. Creates a new file if it doesn’t exist.

---

## Question 2: What is File Reading? Explain with example.

**Answer**:  
File reading in C can be done using functions like `fscanf`, `fgets`, or `fgetc`. Example:
```c
FILE *file = fopen("example.txt", "r");
char line[100];
while (fgets(line, sizeof(line), file)) {
    printf("%s", line);
}
fclose(file);
```

---

## Question 3: What is File Writing? Explain with example.

**Answer**:  
File writing in C can be done using functions like `fprintf`, `fputs`, or `fputc`. Example:
```c
FILE *file = fopen("example.txt", "w");
fprintf(file, "Hello, World!\n");
fclose(file);
```

---

## Question 4: How to create a new file using C language?

**Answer**:  
To create a new file in C, use the `fopen()` function with the mode `"w"` or `"a"`. Example:
```c
FILE *file = fopen("newfile.txt", "w");
if (file == NULL) {
    perror("Error creating file");
} else {
    printf("File created successfully");
    fclose(file);
}
```

---

## Question 5: Explain fclose() function with its importance.

**Answer**:  
The `fclose()` function closes an open file and releases resources associated with it. Example:
```c
FILE *file = fopen("example.txt", "r");
if (file) {
    fclose(file);
}
```
Importance:
- Prevents memory leaks.
- Ensures data is written to the file properly.

---

## Question 6: Explain fgets() function in detail.

**Answer**:  
The `fgets()` function reads a line from a file and stores it in a string. Example:
```c
FILE *file = fopen("example.txt", "r");
char buffer[100];
if (fgets(buffer, sizeof(buffer), file)) {
    printf("Read line: %s", buffer);
}
fclose(file);
```

---

## Question 7: Explain fputs() function in detail.

**Answer**:  
The `fputs()` function writes a string to a file. Example:
```c
FILE *file = fopen("example.txt", "w");
if (file) {
    fputs("Hello, World!\n", file);
    fclose(file);
}
```

---

## Question 8: Explain fwrite() function in detail.

**Answer**:  
The `fwrite()` function writes binary data to a file. Example:
```c
FILE *file = fopen("data.bin", "wb");
int data[] = {1, 2, 3, 4, 5};
if (file) {
    fwrite(data, sizeof(int), 5, file);
    fclose(file);
}
```

---

## Question 9: Explain fread() function in detail.

**Answer**:  
The `fread()` function reads binary data from a file. Example:
```c
FILE *file = fopen("data.bin", "rb");
int data[5];
if (file) {
    fread(data, sizeof(int), 5, file);
    fclose(file);
}
for (int i = 0; i < 5; i++) {
    printf("%d ", data[i]);
}
```

---


# Patterns

## Question 1: Print the following pattern:
```
1 2 3 4 5
1 2 3 4 5
1 2 3 4 5
1 2 3 4 5
1 2 3 4 5
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= 5; j++) {
        printf("%d ", j);
    }
    printf("\n");
}
```

---

## Question 2: Print the following pattern:
```
1
1 2
1 2 3
1 2 3 4
1 2 3 4 5
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", j);
    }
    printf("\n");
}
```

---

## Question 3: Print the following pattern:
```
5
5 4
5 4 3
5 4 3 2
5 4 3 2 1
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 5; j >= i; j--) {
        printf("%d ", j);
    }
    printf("\n");
}
```

---

## Question 4: Print the following pattern:
```
1 2 3 4 5
1 2 3 4
1 2 3
1 2
1
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", j);
    }
    printf("\n");
}
```

---

## Question 5: Print the following pattern:
```
5 4 3 2 1
5 4 3 2
5 4 3
5 4
5
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 5; j >= 6 - i; j--) {
        printf("%d ", j);
    }
    printf("\n");
}
```

---

## Question 6: Print the following pattern:
```
A B C D E
A B C D
A B C
A B
A
```
**Answer**:
```c
for (char ch = 'A'; ch <= 'E'; ch++) {
    for (char c = 'A'; c <= ch; c++) {
        printf("%c ", c);
    }
    printf("\n");
}
```

---

## Question 7: Print the following pattern:
```
A B C D E
B C D E
C D E
D E
E
```
**Answer**:
```c
for (char ch = 'A'; ch <= 'E'; ch++) {
    for (char c = ch; c <= 'E'; c++) {
        printf("%c ", c);
    }
    printf("\n");
}
```

---

## Question 8: Print the following pattern:
```
    *
   ***
  *****
 *******
*********
```
**Answer**:
```c
for (int i = 1; i <= 9; i += 2) {
    for (int j = i; j < 9; j += 2) {
        printf(" ");
    }
    for (int j = 1; j <= i; j++) {
        printf("*");
    }
    printf("\n");
}
```

---

## Question 9: Print the following pattern:
```
*********
 *******
  *****
   ***
    *
```
**Answer**:
```c
for (int i = 9; i >= 1; i -= 2) {
    for (int j = i; j < 9; j += 2) {
        printf(" ");
    }
    for (int j = 1; j <= i; j++) {
        printf("*");
    }
    printf("\n");
}
```

---

## Question 10: Print the following pattern:
```
    *
   ***
  *****
 *******
// ...continue adding all 50 questions and answers in a similar format...
```

## Question 11: Print the following pattern:
```
5 5 5 5 5
5 5 5 5
5 5 5
5 5
5
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
        printf("5 ");
    }
    printf("\n");
}
```

---

## Question 12: Print the following pattern:
```
1
2 2
3 3 3
4 4 4 4
5 5 5 5 5
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", i);
    }
    printf("\n");
}
```

---

## Question 13: Print the following pattern:
```
5
4 4
3 3 3
2 2 2 2
1 1 1 1 1
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= 6 - i; j++) {
        printf("%d ", i);
    }
    printf("\n");
}
```

---

## Question 14: Print the following pattern:
```
1 1 1 1 1
2 2 2 2
3 3 3
4 4
5
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 5; j >= i; j--) {
        printf("%d ", i);
    }
    printf("\n");
}
```

---

## Question 15: Print the following pattern:
```
5 5 5 5 5
4 4 4 4
3 3 3
2 2
1
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", i);
    }
    printf("\n");
}
```

---

## Question 16: Print the following pattern:
```
A A A A A
B B B B B
C C C C C
D D D D D
E E E E E
```
**Answer**:
```c
for (char ch = 'A'; ch <= 'E'; ch++) {
    for (int j = 1; j <= 5; j++) {
        printf("%c ", ch);
    }
    printf("\n");
}
```

---

## Question 17: Print the following pattern:
```
A
A B
A B C
A B C D
A B C D E
```
**Answer**:
```c
for (char ch = 'A'; ch <= 'E'; ch++) {
    for (char c = 'A'; c <= ch; c++) {
        printf("%c ", c);
    }
    printf("\n");
}
```

---

## Question 18: Print the following pattern:
```
E
E D
E D C
E D C B
E D C B A
```
**Answer**:
```c
for (char ch = 'E'; ch >= 'A'; ch--) {
    for (char c = 'E'; c >= ch; c--) {
        printf("%c ", c);
    }
    printf("\n");
}
```

---

## Question 19: Print the following pattern:
```
A B C D E
A B C D
A B C
A B
A
```
**Answer**:
```c
for (char ch = 'E'; ch >= 'A'; ch--) {
    for (char c = 'A'; c <= ch; c++) {
        printf("%c ", c);
    }
    printf("\n");
}
```

---

## Question 20: Print the following pattern:
```
E D C B A
D C B A
C B A
B A
A
```
**Answer**:
```c
for (char ch = 'E'; ch >= 'A'; ch--) {
    for (char c = 'E'; c >= ch; c--) {
        printf("%c ", c);
    }
    printf("\n");
}
```

---

## Question 21: Print the following pattern:
```
A B C D E
B C D E
C D E
D E
E
```
**Answer**:
```c
for (char ch = 'A'; ch <= 'E'; ch++) {
    for (char c = ch; c <= 'E'; c++) {
        printf("%c ", c);
    }
    printf("\n");
}
```

---

## Question 22: Print the following pattern:
```
E D C B A
D C B A
C B A
B A
A
```
**Answer**:
```c
for (char ch = 'E'; ch >= 'A'; ch--) {
    for (char c = 'E'; c >= ch; c--) {
        printf("%c ", c);
    }
    printf("\n");
}
```

---

## Question 23: Print the following pattern:
```
A
A A
A A A
A A A A
A A A A A
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("A ");
    }
    printf("\n");
}
```

---

## Question 24: Print the following pattern:
```
E
E E
E E E
E E E E
E E E E E
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("E ");
    }
    printf("\n");
}
```

---

## Question 25: Print the following pattern:
```
A A A A A
A A A A
A A A
A A
A
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
        printf("A ");
    }
    printf("\n");
}
```

---

## Question 26: Print the following pattern:
```
E E E E E
E E E E
E E E
E E
E
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
        printf("E ");
    }
    printf("\n");
}
```

---

## Question 27: Print the following pattern:
```
A
B B
C C C
D D D D
E E E E E
```
**Answer**:
```c
for (char ch = 'A'; ch <= 'E'; ch++) {
    for (int j = 1; j <= ch - 'A' + 1; j++) {
        printf("%c ", ch);
    }
    printf("\n");
}
```

---

## Question 28: Print the following pattern:
```
E
D D
C C C
B B B B
A A A A A
```
**Answer**:
```c
for (char ch = 'E'; ch >= 'A'; ch--) {
    for (int j = 1; j <= 'E' - ch + 1; j++) {
        printf("%c ", ch);
    }
    printf("\n");
}
```

---

## Question 29: Print the following pattern:
```
A A A A A
B B B B
C C C
D D
E
```
**Answer**:
```c
for (char ch = 'A'; ch <= 'E'; ch++) {
    for (int j = 5; j >= ch - 'A' + 1; j--) {
        printf("%c ", ch);
    }
    printf("\n");
}
```

---

## Question 30: Print the following pattern:
```
E E E E E
D D D D
C C C
B B
A
```
**Answer**:
```c
for (char ch = 'E'; ch >= 'A'; ch--) {
    for (int j = 1; j <= ch - 'A' + 1; j++) {
        printf("%c ", ch);
    }
    printf("\n");
}
```

---

## Question 31: Print the following pattern:
```
* * * * *
* * * * *
* * * * *
* * * * *
* * * * *
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= 5; j++) {
        printf("* ");
    }
    printf("\n");
}
```

---

## Question 32: Print the following pattern:
```
*
* *
* * *
* * * *
* * * * *
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("* ");
    }
    printf("\n");
}
```

---

## Question 33: Print the following pattern:
```
* * * * *
* * * *
* * *
* *
*
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
        printf("* ");
    }
    printf("\n");
}
```

---

## Question 34: Print the following pattern:
```
1 2 3 4 5
6 7 8 9 10
11 12 13 14 15
16 17 18 19 20
21 22 23 24 25
```
**Answer**:
```c
int count = 1;
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= 5; j++) {
        printf("%d ", count++);
    }
    printf("\n");
}
```

---

## Question 35: Print the following pattern:
```
1
2 2
3 3 3
4 4 4 4
5 5 5 5 5
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", i);
    }
    printf("\n");
}
```

---

## Question 36: Print the following pattern:
```
5
4 4
3 3 3
2 2 2 2
1 1 1 1 1
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= 6 - i; j++) {
        printf("%d ", i);
    }
    printf("\n");
}
```

---

## Question 37: Print the following pattern:
```
1 1 1 1 1
2 2 2 2
3 3 3
4 4
5
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 5; j >= i; j--) {
        printf("%d ", i);
    }
    printf("\n");
}
```

---

## Question 38: Print the following pattern:
```
A
A A
A A A
A A A A
A A A A A
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("A ");
    }
    printf("\n");
}
```

---

## Question 39: Print the following pattern:
```
A A A A A
A A A A
A A A
A A
A
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
        printf("A ");
    }
    printf("\n");
}
```

---

## Question 40: Print the following pattern:
```
+
+ -
+ - +
+ - + -
+ - + - +
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf(i % 2 == 0 ? "- " : "+ ");
    }
    printf("\n");
}
```

---

## Question 41: Print the following pattern:
```
+
- -
+ + +
- - - -
+ + + + +
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf(i % 2 == 0 ? "- " : "+ ");
    }
    printf("\n");
}
```

---

## Question 42: Print the following pattern:
```
1
0 1
1 0 1
0 1 0 1
1 0 1 0 1
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", (i + j) % 2);
    }
    printf("\n");
}
```

---

## Question 43: Print the following pattern:
```
0 1 0 1 0
1 0 1 0
0 1 0
1 0
0
```
**Answer**:
```c
for (int i = 5; i >= 1; i--) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", (i + j) % 2);
    }
    printf("\n");
}
```

---

## Question 44: Print the following pattern:
```
@
# #
@ @ @
# # # #
@ @ @ @ @
```
**Answer**:
```c
for (int i = 1; i <= 5; i++) {
    for (int j = 1; j <= i; j++) {
        printf(i % 2 == 0 ? "# " : "@ ");
    }
    printf("\n");
}
```

---

## Question 45: Print the following pattern:
```
HP1
HP2 HP2
HP3 HP3 HP3
HP4 HP4 HP4 HP4
```
**Answer**:
```c
for (int i = 1; i <= 4; i++) {
    for (int j = 1; j <= i; j++) {
        printf("HP%d ", i);
    }
    printf("\n");
}
```

---

## Question 46: Print the following pattern:
```
D P D P D P D P
D P D P D P
D P D P
D P
```
**Answer**:
```c
for (int i = 4; i >= 1; i--) {
    for (int j = 1; j <= i * 2; j++) {
        printf(j % 2 == 0 ? "P " : "D ");
    }
    printf("\n");
}
```

---

## Question 47: Print the following pattern:
```
1
2 3
4 5 6
7 8 9 10
```
**Answer**:
```c
int count = 1;
for (int i = 1; i <= 4; i++) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", count++);
    }
    printf("\n");
}
```

---

## Question 48: Print the following pattern:
```
1
2 4
3 6 9
4 8 12 16
```
**Answer**:
```c
for (int i = 1; i <= 4; i++) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", i * j);
    }
    printf("\n");
}
```

---

## Question 49: Print the following pattern:
```
1
1 0
1 0 1
1 0 1 0
```
**Answer**:
```c
for (int i = 1; i <= 4; i++) {
    for (int j = 1; j <= i; j++) {
        printf("%d ", j % 2);
    }
    printf("\n");
}
```

---

## Question 50: Print the following pattern:
```
*
* *
* * *
* * * *
```
**Answer**:
```c
for (int i = 1; i <= 4; i++) {
    for (int j = 1; j <= i; j++) {
        printf("* ");
    }
    printf("\n");
}
```
