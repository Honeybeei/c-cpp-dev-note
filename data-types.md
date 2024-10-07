# 🔢 Data Types

- [🔢 Data Types](#-data-types)
  - [🤔 What is Data Type?](#-what-is-data-type)
  - [📝 Types of Data Types](#-types-of-data-types)
    - [Primitive Data Types](#primitive-data-types)
    - [Derived Data Types](#derived-data-types)
    - [User-defined Data Types](#user-defined-data-types)
  - [📚 About data type modifier](#-about-data-type-modifier)

## 🤔 What is Data Type?

Data types are used to define the type of data a variable can hold. Let's think of a variable as a box that can hold some value. The type of the box determines what kind of value it can hold. For example, a box can hold a number, a character, a string, etc. The type of the box is the data type.

## 📝 Types of Data Types

There are three types of data types.

### Primitive Data Types

Primitive Data Types are the basic data types that are provided by the programming language. They are used for representing simple values. The primitive data types are:

- `int`: For representing integer numbers.
- `char`: For representing characters.
- `float`: For representing floating-point numbers.
- `double`: For representing double-precision floating-point numbers.
- `void`: For representing no value.
- `bool` (C++ only): For representing boolean values.
- `wchar_t` (C++ only): For representing wide characters.

```cpp
int a = 10;
char b = 'A';
float c = 3.14;
double d = 3.14159;
void print_smt() {
    cout << "Hello, World!" << endl;
} // Return no value
bool is_true = true;
wchar_t wc = L'あ';
```

### Derived Data Types

Derived Data Types are the data types that are derived from the primitive data types. They are used for representing complex values. The derived data types are:

- `array`: For representing a collection of values of the same type.
- `pointer`: For representing the memory address of a variable.
- `function`: For representing a function.
- `reference` (C++ only): For representing an alias to a variable.

```cpp
int arr[5] = {1, 2, 3, 4, 5};
int *ptr = &a;
int sum(int a, int b) {
    return a + b;
}
int &ref = a;
```

### User-defined Data Types

User-defined Data Types are the data types that are defined by the user. They are used for representing custom values. The user-defined data types are:

- `struct`: For representing a collection of values of different types.
- `union`: For representing a collection of values that share the same memory location.
- `enum`: For representing a set of named integer constants.
- `typedef`: For defining an alias for a data type.
- `class` (C++ only): For representing a collection of values and functions.

```cpp
struct Point {
    int x;
    int y;
};

union Number {
    int i;
    float f;
};

enum Color {
    RED,
    GREEN,
    BLUE
};

typedef int Number;

class Circle {
    int radius;
    float area() {
        return 3.14 * radius * radius;
    }
};

```

## 📚 About data type modifier

Data type modifiers are used to modify the properties of a data type.

```c
int a; // int data type
unsigned int b; // unsigned int data type
long int c; // long int data type
```

We will handle this topic in more detail in the [next section](./modifiers-type-qualifiers.md).
