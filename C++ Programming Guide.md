# C++ Programming Guide 🚀
*A comprehensive guide to core programming concepts*

## 📘 Program Structure

### Basic Program Template
```cpp
#include <iostream>
using namespace std;

int main() {
    // Your code goes here
    return 0;
}
```

### Key Components Explained
- 🔹 `#include <iostream>`: Header for input/output operations
- 🔹 `using namespace std`: Makes std members directly accessible
- 🔹 `int main()`: Entry point of program
- 🔹 `return 0`: Indicates successful program completion

## 📝 Comments

### Types of Comments
```cpp
// Single-line comment

/* Multi-line comment
   Can span multiple lines
   Used for longer explanations */
```

### Best Practices
- ✅ Use comments to explain complex logic
- ✅ Keep comments updated with code changes
- ✅ Write clear, concise comments

## 🔢 Data Types

### Fundamental Data Types Table

| Type | Size | Range | Example |
|------|------|--------|---------|
| `int` | 4 bytes | -2³¹ to 2³¹-1 | `int age = 25;` |
| `long long` | 8 bytes | -2⁶³ to 2⁶³-1 | `long long population = 7800000000;` |
| `float` | 4 bytes | ~7 decimal digits | `float price = 99.99f;` |
| `double` | 8 bytes | ~15 decimal digits | `double pi = 3.14159265359;` |
| `char` | 1 byte | -128 to 127 | `char grade = 'A';` |
| `bool` | 1 byte | true/false | `bool isActive = true;` |

## 📝 Variable Declaration

### Syntax Options
```cpp
// Method 1: Declaration only
int number;

// Method 2: Declaration with initialization
int age = 25;

// Method 3: Multiple declarations
int x = 1, y = 2, z = 3;
```

### Initialization Best Practices
- ✅ Always initialize variables before use
- ✅ Use meaningful variable names
- ✅ Follow variable naming rules

## C++ Variable Naming Rules and Best Practices 📝

### 🚫 Rules: What You Cannot Do

```cpp
// ❌ INVALID Variable Names
int 123num;        // Cannot start with a number
int my name;       // Cannot contain spaces
int my-score;      // Cannot use hyphens
int for;           // Cannot use reserved keywords
int class;         // Cannot use reserved keywords
int my#variable;   // Cannot use special characters (except _)
```

### ✅ Rules: What You Can Do

```cpp
// ✅ VALID Variable Names
int number123;     // Can contain numbers (not at start)
int _score;        // Can start with underscore
int myScore;       // Can use camelCase
int my_score;      // Can use snake_case
int score1;        // Can end with numbers
int numberOfStudents;  // Can be descriptive
```

### 🔑 Reserved Keywords
Cannot use these as variable names:
```cpp
auto     break    case     char      const    continue
default  do       double   else      enum     extern
float    for      goto     if        int      long
register return   short    signed    sizeof   static
struct   switch   typedef  union     unsigned void
volatile while    bool     catch     class    const_cast
delete   dynamic_cast      explicit  false    friend
inline   mutable  namespace new      operator private
protected public  reinterpret_cast   static_cast      template
this     throw    true     try       typeid   typename
using    virtual  wchar_t
```

## 📚 String Operations

### String Basics
```cpp
string name = "John";
string fullName = name + " Doe";  // Concatenation
int length = name.length();       // String length
```

## ➗ Operators

### Arithmetic Operators
```cpp
int a = 10, b = 3;
int sum = a + b;        // Addition (13)
int diff = a - b;       // Subtraction (7)
int product = a * b;    // Multiplication (30)
int quotient = a / b;   // Division (3)
int remainder = a % b;  // Modulus (1)
```

### Example with Mixed Types
```cpp
double x = 5.0;
int y = 2;
double result = x / y;  // Results in 2.5
```

## 🔄 Modulus Operations

### Common Uses
```cpp
// Get last digit
int lastDigit = number % 10;

// Circular rotation (0-359 degrees)
int angle = 400 % 360;  // Returns 40
```

## 🔀 Assignment Operators
```cpp
int x = 10;
x += 5;  // x = 15
x -= 3;  // x = 12
x *= 2;  // x = 24
x /= 4;  // x = 6
x %= 4;  // x = 2
```

## ⬆️ Increment/Decrement

### Prefix vs Postfix
```cpp
int a = 5;
int b = ++a;  // a = 6, b = 6 (prefix)
int c = a++;  // c = 6, a = 7 (postfix)
```

## 📥 Input/Output

### Basic Input
```cpp
int age;
string name;

cout << "Enter your first name: ";
cin >> name; // Mohamed

cout << "Enter your age: ";
cin >> age;
```

Or

```cpp
int age;
string name;

cin >> name >> age;
```
-----

```cpp
string name;

cout << "Enter your full name: ";
getline(cin, name); // Mohamed Ali
```

### Formatted Output
```cpp
cout << "Name: " << name << "\n";
cout << "Age: " << age << "\t";
```

Or

```cpp
cout << "Name: " << name << "\n" << "Age: " << age << "\t";
```

### Special Characters
- `\n`: Newline
- `\t`: Tab
- `\\`: Backslash
- `\"`: Double quote

## 🎯 Practice Problems

### Problem 1: Temperature Converter
```cpp
double celsius;
cout << "Enter temperature in Celsius: ";
cin >> celsius;
double fahrenheit = (celsius * 9/5) + 32;
cout << celsius << "°C = " << fahrenheit << "°F\n";
```

## 📌 Quick Tips

1. 💡 Always initialize variables
2. 💡 Use meaningful variable names
3. 💡 Comment complex logic
5. 💡 Format output for readability

## 🔍 Debug Techniques

1. Use step-by-step execution
2. Check for common errors:
   - Missing semicolons
   - Uninitialized variables
   - Integer division when float needed
   - Off-by-one errors

---
