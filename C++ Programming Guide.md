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
- ✅ Follow consistent naming conventions

## 📚 String Operations

### String Basics
```cpp
string name = "John";
string fullName = name + " Doe";  // Concatenation
int length = name.length();       // String length
```

### Common String Operations
```cpp
string text = "Hello World";
text.substr(0, 5);      // Returns "Hello"
text.find("World");     // Returns position 6
text[0];               // Returns 'H'
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
// Check if number is even
if (number % 2 == 0) {
    cout << "Even number";
}

// Get last digit
int lastDigit = number % 10;

// Circular rotation (0-359 degrees)
int angle = 400 % 360;  // Returns 40
```

## 🔀 Compound Assignment
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

cout << "Enter your name: ";
getline(cin, name);

cout << "Enter your age: ";
cin >> age;
```

### Formatted Output
```cpp
cout << "Name: " << name << "\n";
cout << "Age: " << age << "\t";
cout << fixed << setprecision(2);
cout << "Price: $" << price << endl;
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

### Problem 2: Number Analyzer
```cpp
int number;
cout << "Enter a number: ";
cin >> number;

cout << "Properties of " << number << ":\n";
cout << "Even/Odd: " << (number % 2 == 0 ? "Even" : "Odd") << "\n";
cout << "Positive/Negative: " << (number > 0 ? "Positive" : number < 0 ? "Negative" : "Zero") << "\n";
```

## 📌 Quick Tips

1. 💡 Always initialize variables
2. 💡 Use meaningful variable names
3. 💡 Comment complex logic
4. 💡 Test edge cases
5. 💡 Format output for readability

## 🔍 Debug Techniques

1. Print variable values at key points
2. Use step-by-step execution
3. Check for common errors:
   - Missing semicolons
   - Uninitialized variables
   - Integer division when float needed
   - Off-by-one errors

---
