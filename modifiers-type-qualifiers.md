# 📝 Modifiers and Type Qualifiers

- [📝 Modifiers and Type Qualifiers](#-modifiers-and-type-qualifiers)
  - [🛠️ Modifiers](#️-modifiers)
    - [`signed` and `unsigned`](#signed-and-unsigned)
    - [`short` and `long`](#short-and-long)
    - [Table of Data Types](#table-of-data-types)
  - [🔒 Type Qualifiers](#-type-qualifiers)
    - [`const`](#const)
    - [`volatile`](#volatile)
    - [`restrict` (C99. C++ does not have `restrict`)](#restrict-c99-c-does-not-have-restrict)
    - [`mutable` (C++ only)](#mutable-c-only)
    - [`constexpr` (C++11)](#constexpr-c11)
  - [🛡️ Storage Class Specifiers](#️-storage-class-specifiers)
    - [`auto` (C++11)](#auto-c11)
    - [`register`](#register)
    - [`static`](#static)
    - [`extern`](#extern)

> Q: What are the modifiers and type qualifiers in C and C++?
>
> A: Modifiers and type qualifiers provide additional information about how variables are stored and used.

## 🛠️ Modifiers

Modifiers change the meaning of the base data types.

### `signed` and `unsigned`

- `signed`: Indicates that the variable can store both positive and negative values.
- `unsigned`: Indicates that the variable can store only positive values.

```cpp
int x = -10; // signed integer. Default is signed
signed int y = -10; // signed integer
unsigned int z = 10; // unsigned integer
// unsigned int w = -10; // Error: unsigned integer cannot store negative values
```

### `short` and `long`

- `short`: Reduces the size of the variable, which may save memory but reduce the range of values.
- `long`: Increases the size of the variable, which may increase the range of values but use more memory.

```cpp
short int x = 10; // short integer
long int y = 100000L; // long integer
```

### Table of Data Types

| Data Type            | Size (bytes)       | Minimum Value                              | Maximum Value                              |
|----------------------|--------------------|--------------------------------------------|--------------------------------------------|
| `char`               | 1                  | -128                                       | 127                                        |
| `unsigned char`      | 1                  | 0                                          | 255                                        |
| `short`              | 2                  | -32,768                                    | 32,767                                     |
| `unsigned short`     | 2                  | 0                                          | 65,535                                     |
| `int`                | 4                  | -2,147,483,648                             | 2,147,483,647                              |
| `unsigned int`       | 4                  | 0                                          | 4,294,967,295                              |
| `long`               | 4 (32-bit)         | -2,147,483,648                             | 2,147,483,647                              |
|                      | 8 (64-bit)         | -9,223,372,036,854,775,808                 | 9,223,372,036,854,775,807                  |
| `unsigned long`      | 4 (32-bit)         | 0                                          | 4,294,967,295                              |
|                      | 8 (64-bit)         | 0                                          | 18,446,744,073,709,551,615                 |
| `long long`          | 8                  | -9,223,372,036,854,775,808                 | 9,223,372,036,854,775,807                  |
| `unsigned long long` | 8                  | 0                                          | 18,446,744,073,709,551,615                 |
| `float`              | 4                  | 1.2E-38                                    | 3.4E+38                                    |
| `double`             | 8                  | 2.3E-308                                   | 1.7E+308                                   |
| `long double`        | 8 (x86-64 Windows) | 2.3E-308                                   | 1.7E+308                                   |
|                      | 16 (x86-64 Linux/macOS) | 3.4E-4932                             | 1.1E+4932                                  |
| `wchar_t`            | 2 (Windows)        | 0                                          | 65,535                                     |
|                      | 4 (Linux/macOS)    | 0                                          | 4,294,967,295                              |

## 🔒 Type Qualifiers

Type qualifiers provide additional properties to a variable's type, restricting how it can be used.

### `const`

- `const`: Indicates that the variable's value cannot be changed after initialization.

```cpp
const int x = 10; // x is a constant
// x = 20; // Error: x is a constant and cannot be changed
```

### `volatile`

- `volatile`: Tells the compiler not to optimize the variable, as it may change unexpectedly by external factors (such as hardware or another thread).

```cpp
volatile int x = 10; // x is volatile
```

### `restrict` (C99. C++ does not have `restrict`)

- `restrict`: Used for pointers, it indicates that the pointer is the only way to access the object it points to. This allows the compiler to optimize better.

```c
void foo(int* restrict a, int* restrict b) {
    *a = 10;
    *b = 20;
}
```

### `mutable` (C++ only)

- `mutable`: Used in classes and structures, it allows a member variable to be modified even if the containing object is `const`.

```cpp
class A {
public:
    mutable int x;
    A() : x(0) {}
};

const A obj;
obj.x = 10; // Allowed because x is mutable
```

### `constexpr` (C++11)

- `constexpr`: Indicates that the value of the variable is constant and can be evaluated at compile time.

```cpp
constexpr int x = 10 + 20; // x = 30 and it will be evaluated at compile time
```

## 🛡️ Storage Class Specifiers

### `auto` (C++11)

- `auto`: Automatically deduces the type of the variable from its initializer.

```cpp
auto x = 10; // x is an integer
```

### `register`

- `register`: Suggests the compiler to store the variable in a register for faster access.

```cpp
register int x = 10; // x is stored in a register
```

### `static`

- `static`: Extends the lifetime of the variable to the entire program execution.

```cpp
void foo() {
    static int x = 0; // x is initialized only once
    x++;
    cout << x << endl;
}

foo(); // 1
foo(); // 2
foo(); // 3
```

### `extern`

- `extern`: Declares a variable that is defined in another file.

```cpp
// file1.cpp
int x = 10;

// file2.cpp
extern int x; // x is defined in file1.cpp
```
