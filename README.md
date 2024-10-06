# 🙋 C and C++

I started learning C and C++ because projects from 42 Seoul required me to learn these languages. C and C++ are powerful programming languages widely used for system software, application development, high-performance computing, and embedded systems. They offer low-level memory manipulation capabilities and are essential for understanding how software interacts with hardware.

## 🎯 Purpose of this Dev Note

The purpose of this Dev Note is to serve as a practical reference guide for myself and others who may need a quick refresher on specific concepts in C and C++. It consolidates essential topics, code snippets, and explanations that can be easily accessed when needed. By organizing the information into structured markdown files, it becomes a handy cheat sheet that aids in efficient learning and development.

## 🌐 Overview of C and C++

C is a procedural programming language developed in the early 1970s. It provides low-level access to memory and offers a minimalistic set of keywords, making it suitable for system programming, embedded systems, and performance-critical applications.

C++, developed as an extension of C, introduces object-oriented programming features, generic programming through templates, and additional standard libraries. It retains compatibility with C while offering higher-level abstractions, making it suitable for complex software development, game development, and applications requiring both performance and abstraction.

## 🔍 Key Differences between C and C++

| Feature              | C                              | C++                                    |
|----------------------|--------------------------------|----------------------------------------|
| Programming Paradigm | Procedural                     | Procedural & Object-Oriented           |
| Standard Libraries   | Smaller                        | Rich Standard Template Library (STL)   |
| Memory Management    | Manual (`malloc`, `free`)      | `new`, `delete`, Smart Pointers        |
| Features             | Functions, Structures          | Classes, Inheritance, Templates, etc.  |
| Compatibility        | -                              | Backward-compatible with most of C     |

## 📑 List of Contents

### 🛠️ Basics (Common to Both C and C++)

- [x] [Hello World in C and C++](./hello-world.md): Main function, comments, and printing output in both languages.
- [ ] [Data Types](./data-types.md): Primitive data types in both languages.
- [ ] [Modifiers and Type Qualifiers](./modifiers-type-qualifiers.md): Using `signed`, `unsigned`, `short`, `long`, `const`, and `volatile`.
- [ ] [Variables and Constants](./variables-constants.md): Declaring and using variables and constants.
- [ ] [Scope and Lifetime of Variables](./scope-lifetime.md): Understanding variable scope and duration.
- [ ] [Operators](./operators.md): Arithmetic, relational, logical, and bitwise operators.
- [ ] [Type Casting](./type-casting.md): Implicit and explicit type conversions.
- [ ] [Control Flow](./control-flow.md): Conditional statements, loops, and jump statements.
- [ ] [Functions](./functions.md): Defining and calling functions.
- [ ] [Arrays](./arrays.md): Declaring and using arrays.
- [ ] [Strings](./strings.md): Handling strings.
- [ ] [Pointers](./pointers.md): Understanding pointers and their usage.

### 🚀 Intermediate Topics

#### C Specific Features

- [ ] [Preprocessor Directives](./c/preprocessor-directives.md): Using preprocessor directives in C.
- [ ] [Macros and Macro Functions](./c/macros.md): Defining and using macros.
- [ ] [Dynamic Memory Allocation in C](./c/dynamic-memory-allocation.md): Using `malloc`, `calloc`, `realloc`, and `free`.
- [ ] [Structures and Unions](./c/structures-unions.md): Defining and using structures and unions.
  - [ ] [Bit Fields in Structures](./c/bit-fields.md): Defining and using bit fields.
- [ ] [Enums and Typedef](./c/enums-typedef.md): Enumerations and type definitions.
- [ ] [Variable Argument Functions](./c/variable-arguments.md): Using `stdarg.h` for functions with variable arguments.
- [ ] [File Input/Output in C](./c/file-io.md): Reading from and writing to files.
- [ ] [Command Line Arguments](./c/command-line-arguments.md): Handling command-line arguments in C programs.

#### C++ Specific Features

- [ ] [Namespaces](./cpp/namespaces.md): Defining and using namespaces.
- [ ] [Input/Output in C++](./cpp/input-output.md): Using streams for input and output.
- [ ] [References](./cpp/references.md): Understanding references.
- [ ] [Function Overloading and Default Arguments](./cpp/function-overloading.md): Using overloaded functions and default parameters.
- [ ] [Inline Functions](./cpp/inline-functions.md): Improving performance with inline functions.
- [ ] [Dynamic Memory Allocation in C++](./cpp/dynamic-memory-allocation.md): Using `new` and `delete`.
- [ ] [Strongly Typed Enums](./cpp/strongly-typed-enums.md): Using `enum class` (C++11).
- [ ] [Type Inference with `auto`](./cpp/auto.md): Using `auto` for type deduction (C++11).
- [ ] [Constants and `constexpr`](./cpp/constexpr.md): Compile-time constants (C++11).
- [ ] [Nullptr Keyword](./cpp/nullptr.md): Using `nullptr` instead of `NULL` (C++11).
- [ ] [Range-Based For Loops](./cpp/range-based-for.md): Simplifying loops with range-based `for` (C++11).

### 🏛️ Object-Oriented Programming in C++

- [ ] [Classes and Objects](./cpp/classes-objects.md): Defining classes and creating objects.
- [ ] [Access Specifiers](./cpp/access-specifiers.md): Understanding `public`, `protected`, and `private`.
- [ ] [Constructors and Destructors](./cpp/constructors-destructors.md): Initializing and cleaning up objects.
- [ ] [Copy and Move Constructors](./cpp/copy-move-constructors.md): Copying and moving objects (C++11).
- [ ] [Inheritance](./cpp/inheritance.md): Implementing inheritance.
- [ ] [Polymorphism](./cpp/polymorphism.md): Understanding polymorphism and virtual functions.
- [ ] [Virtual Destructors](./cpp/virtual-destructors.md): Ensuring proper cleanup in inheritance hierarchies.
- [ ] [Abstract Classes and Interfaces](./cpp/abstract-classes.md): Using pure virtual functions.
- [ ] [Operator Overloading](./cpp/operator-overloading.md): Overloading operators for custom classes.
- [ ] [Friend Classes and Functions](./cpp/friend.md): Granting access to private members.
- [ ] [Static Members](./cpp/static-members.md): Class-level variables and functions.
- [ ] [The `this` Pointer](./cpp/this-pointer.md): Understanding the `this` pointer.
- [ ] [Templates in C++](./cpp/templates.md): Using templates for generic programming.

### 🧠 Advanced Topics

#### C Advanced Topics

- [ ] [Bit Manipulation](./c/bit-manipulation.md): Performing bitwise operations.
- [ ] [Memory Management Best Practices in C](./c/memory-management.md): Tips for efficient memory management.
- [ ] [Debugging Techniques in C](./c/debugging.md): Using tools like GDB.
- [ ] [Testing and Test Cases in C](./c/testing.md): Writing unit tests for C code.
- [ ] [Dealing with Undefined Behavior](./c/undefined-behavior.md): Understanding and avoiding undefined behavior.
- [ ] [Multi-file Projects in C](./c/multi-file-projects.md): Organizing C code into multiple files.

#### C++ Advanced Topics

- [ ] [Exception Handling](./cpp/exception-handling.md): Handling exceptions in C++ programs.
- [ ] [Smart Pointers](./cpp/smart-pointers.md): Using `std::unique_ptr`, `std::shared_ptr`, `std::weak_ptr` (C++11).
- [ ] [Move Semantics and Rvalue References](./cpp/move-semantics.md): Efficient object transfer (C++11).
- [ ] [Perfect Forwarding](./cpp/perfect-forwarding.md): Forwarding arguments to other functions (C++11).
- [ ] [Variadic Templates](./cpp/variadic-templates.md): Templates with variable numbers of arguments (C++11).
- [ ] [Type Traits and SFINAE](./cpp/type-traits.md): Compile-time type information.
- [ ] [Compile-Time Programming with `constexpr`](./cpp/constexpr-functions.md): Functions evaluated at compile time.
- [ ] [Lambda Expressions](./cpp/lambda-expressions.md): Defining anonymous functions (C++11).
- [ ] [Function Objects (Functors)](./cpp/functors.md): Using objects as functions.
- [ ] [STL Containers](./cpp/stl-containers.md): Overview of Standard Template Library containers.
- [ ] [STL Iterators](./cpp/stl-iterators.md): Understanding iterators in C++.
- [ ] [STL Algorithms](./cpp/stl-algorithms.md): Using algorithms from the standard library.
- [ ] [Multithreading and Concurrency](./cpp/multithreading.md): Creating multithreaded applications.
- [ ] [Atomic Operations and Memory Model](./cpp/atomic-operations.md): Thread-safe operations and memory model.
- [ ] [Regular Expressions](./cpp/regex.md): Using the `<regex>` library (C++11).
- [ ] [Filesystem Library](./cpp/filesystem.md): File operations with `<filesystem>` (C++17).
- [ ] [Random Number Generation](./cpp/random.md): Using the `<random>` library.
- [ ] [Time Utilities](./cpp/chrono.md): Using the `<chrono>` library.
- [ ] [Thread Support Library](./cpp/thread.md): Multithreading with `<thread>`, `<mutex>`, `<future>`, etc.
- [ ] [Modern C++ Practices](./cpp/modern-cpp-practices.md): Using modern C++ features effectively.

### 📝 Best Practices and Coding Standards

- [ ] [Code Formatting and Style Guidelines](./code-formatting.md): Writing clean and readable code.
- [ ] [The Rule of Three, Five, and Zero](./cpp/rule-of-three-five-zero.md): Managing resources in classes.
- [ ] [RAII (Resource Acquisition Is Initialization)](./cpp/raii.md): Managing resources efficiently.
- [ ] [Memory Management Best Practices](./memory-management.md): Tips for efficient memory management.
- [ ] [Exception Safety in C++](./cpp/exception-safety.md): Writing exception-safe code.
- [ ] [Debugging Techniques](./debugging.md): Tools and techniques for debugging.
- [ ] [Testing and Test Cases](./testing.md): Writing unit tests and test cases.
- [ ] [Writing Portable Code](./portable-code.md): Ensuring code runs across different platforms.
- [ ] [Dealing with Undefined Behavior](./undefined-behavior.md): Understanding and avoiding undefined behavior.
- [ ] [Writing Clean and Maintainable Code](./clean-code.md): Best practices for code quality.
- [ ] [Multi-file Projects](./multi-file-projects.md): Organizing code into multiple files.

### 📎 Appendices

- [ ] [C Standard Library Overview](./c/standard-library.md): Overview of C standard library functions.
  - [ ] [Standard Input/Output `stdio.h`](./c/stdio.md)
  - [ ] [Standard Utilities `stdlib.h`](./c/stdlib.md)
  - [ ] [Math Functions `math.h`](./c/math.md)
  - [ ] [String Functions `string.h`](./c/string.md)
  - [ ] [Time Functions `time.h`](./c/time.md)
  - [ ] [Character Functions `ctype.h`](./c/character.md)
  - [ ] [Error Handling with `errno.h`](./c/errno.md)
- [ ] [C++ Standard Library Overview](./cpp/standard-library.md): Overview of C++ standard library components.
- [ ] [C++ Standards and Features](./cpp/standards.md): Overview of C++11, C++14, C++17, and C++20 features.
- [ ] [Design Patterns in C++](./cpp/design-patterns.md): Implementing common design patterns.
- [ ] [Common Pitfalls and How to Avoid Them](./common-pitfalls.md): Avoiding common errors in programming.
- [ ] [Interfacing with Other Languages](./interfacing.md): Using C/C++ with other languages.
