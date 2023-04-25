# C++ Environment

## History of C
C++ was developed from C. C was developed at the same time as UNIX. 

## History of C++
Adds object-oriented and generic programming construct to C.
Standards of C++ are:
- C++98
- C++03
- C++oX (2011)

C++ requires memory management.

## What makes the C/C++ Program
With C/C++ program we want to make executable Program.
C/C++ code is divided into:
- source files: will contain the actual bodies of the functions.
- header files: willl contain only the declaration of the functions. Header files contain common informations.

## Steps for a C/C++ Program
- Create header and source files;
- Use compiler to translate the code;
- Link the compiled code into a executable file;
- Run the program;

What is a compiler and what is a linker?

The process of executing a C/C++ code is:
1. Source code of file is processed;
2. The processed source files is put in a compiler.
3. The compiler compiles the source files into Object Files, which are machine readable code.
4. All the object files (originated from different source files) are brought together in the linker, which can include libraries from outside.]
5. The objects files in linker builds an executable program.

In C++/C the definition of what will be used as compiler and what will be used as linker is manual.

When the code is wrong, there will be a compiler error and the code will not be transformed in an "object file".
When libraries are missing, there will be an error in the "Linker".

## Structure of C/C++ Source
Consists of functions and variables.

## Example
```
#include <stdio.h>

void main()
{
    printf("This is one line of text\n")
}
```

The `void` is used to specify that it does not return anything: it just does something.
The `#include <stdio.h>` is used to import the header file.

The `printf` is a part of the `<stdio.h>`.

Some remarks:
- comments starts with: /*
- ends with: */
- no nested comments
- can be placed where whitespace is allowed
- in C++ single line comment with: //

The compiler will after remove the whitespace and comments.

Overall, the function must say what type of data it will return. For instance, the following is used to return an "int":
```
int main()
{
    // ...

    return 0;
}
```

## Simple printf() Statements
Printing text:
```
printf("String")
```
Printing values:
```
printf("V1: %d, V2: %f", 10, 30.0)
```
The last prints 10 in decimal form, and 30.0 in the percentage form.

## Quiz
1. What are the advantages of defining separate header and source files?
Larger systems require better separation.

## Code
```
// Preprocessor for include files
#include <stdio.h>          // C style I/O
#include <iostream>         // C++ style I/O using operator overloading
using namespace std;        // The C++ logical collection of functions

void hello_C()
{
    printf("Hello Quantnet, C style\n");
}

void hello_CPP()
{
    cout << "Hello Quantnet, C++ style \n";
}
```

The difference between the two functions is that one uses C and the other uses C++ style.
The "cout" is part of the std::iostream, the "printf" is part of the stdio.h.

The "<>" means system libraries.

"namespace" is our logical collections of functions.








