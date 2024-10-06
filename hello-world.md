# 🙋 Hello World!

- [🙋 Hello World!](#-hello-world)
  - [🔭 Overview](#-overview)
    - [Steps for C](#steps-for-c)
    - [Steps for C++](#steps-for-c-1)
  - [🚀 Let's get started!](#-lets-get-started)
    - [In C](#in-c)
    - [In C++](#in-c-1)
  - [🏄‍♀️ Deep dive](#️-deep-dive)
    - [`#include` directive](#include-directive)
    - [`main` function and code block](#main-function-and-code-block)
    - [Printing `Hello, World!` to the console](#printing-hello-world-to-the-console)
    - [`return 0;` statement](#return-0-statement)
  - [🎉 Congratulations!](#-congratulations)

## 🔭 Overview

We will write a simple program that prints `Hello, World!` to the console. First, just follow the steps, and then we will deep dive into each steps.

### Steps for C

1. We will create a file named `hello.c` and write the code in C.
2. Compile the code using the `gcc` compiler.
3. Run the compiled code.

### Steps for C++

1. We will create a file named `hello.cpp` and write the code in C++.
2. Compile the code using the `g++` compiler.
3. Run the compiled code.

## 🚀 Let's get started!

### In C

Create a file named `hello.c` and write the following code:

```c
// hello.c
#include <stdio.h>

int main(void) {
  printf("Hello, World!\n");
  return 0;
}
```

Compile the code using the following command:

```bash
gcc hello.c -o hello
```

Run the compiled code:

```bash
./hello # Output: Hello, World!
```

### In C++

Create a file named `hello.cpp` and write the following code:

```cpp
// hello.cpp
#include <iostream>

int main() {
  std::cout << "Hello, World!" << std::endl;
  return 0;
}
```

Compile the code using the following command:

```bash
g++ hello.cpp -o hello
```

Run the compiled code:

```bash
./hello # Output: Hello, World!
```

## 🏄‍♀️ Deep dive

Let's check the hello.c and hello.cpp files.

```c
#include <stdio.h>

int main(void) { 
  printf("Hello, World!\n");
  return 0;
}
```

```cpp
#include <iostream>

int main() {
  std::cout << "Hello, World!" << std::endl;
  return 0;
}
```

### `#include` directive

Let's check the first line of both files.

- `#include` is a preprocessor directive that tells the compiler to include the specified header file in the program. Header files contain declarations of functions and variables that are used in the program.
- `<stdio.h>` is a standard input-output library in C. It provides functions like `printf` and `scanf` to read and write data to the console.
- `<iostream>` is a standard input-output library in C++. It provides objects like `std::cout` and `std::cin` to read and write data to the console.

So the first line of both files includes the necessary input-output library for the respective programming language.

> Q: 🤔 What is library?
> A: A library is a collection of precompiled functions and classes that can be used in a program. Libraries provide reusable code that can be used to perform common tasks without having to write the code from scratch. We will check more about libraries([C standard library](./c/standard-library.md) and [C++ standard library](./cpp/standard-library.md)) in the future.

### `main` function and code block

Let's check the `main` function in both files.

- `int main(void)`is the entry point of our program. The `main` function is called when the program is executed. The `int` before `main` indicates that the function will return an integer value. The `void` inside the parentheses indicates that the function does not take any arguments. You can also write `int main()` in C++.
- `{` and `}` are used to define the scope of the function. All the code inside the curly braces is part of the `main` function. The instructions inside the function are executed sequentially from top to bottom when the main function is called.

### Printing `Hello, World!` to the console

Let's check the `printf` and `std::cout` statements in both files.

- `printf("Hello, World!\n");` is a function in C that prints the specified string to the console. The `\n` at the end of the string is an escape sequence that represents a newline character. It moves the cursor to the next line after printing the string.
- `std::cout << "Hello, World!" << std::endl;` is an object in C++ that is used to print the specified string to the console. The `<<` operator is used to insert the string into the `std::cout` object. The `std::endl` is a manipulator that represents a newline character. It moves the cursor to the next line after printing the string.

### `return 0;` statement

Let's check the `return 0;` statement in both files.

- `return 0;` is a statement that returns an integer value from the `main` function. The `0` indicates that the program executed successfully. If the program encounters an error, you can return a non-zero value to indicate the error code.

## 🎉 Congratulations!

That's it! You have successfully written and executed a simple `Hello, World!` program in C and C++. Before moving on, I highly recommend you to play around with the code and try different variations. Happy coding! 🚀
