# 🔄 Boolean Operations & Conditions

### Boolean Values
```cpp
bool isTrue = true;
bool isFalse = false;
```

### Comparison Operators
```cpp
int a = 5, b = 10;
bool isEqual = (a == b);      // false
bool notEqual = (a != b);     // true
bool isGreater = (a > b);     // false
bool isLess = (a < b);        // true
bool greaterEqual = (a >= b); // false
bool lessEqual = (a <= b);    // true
```

### Logical Operators
```cpp
bool x = true, y = false;
bool andResult = x && y;  // false (AND)
bool orResult = x || y;   // true (OR)
bool notResult = !x;      // false (NOT)
```

## 🔀 Conditional Statements

### If Statement
```cpp
int age = 18;

if (age >= 18) {
    cout << "You are an adult\n";
}
```

### If-Else Statement
```cpp
int score = 75;

if (score >= 60) {
    cout << "You passed!\n";
} else {
    cout << "You failed.\n";
}
```

### If-Else If-Else Chain
```cpp
int grade = 85;

if (grade >= 90) {
    cout << "A Grade\n";
} else if (grade >= 80) {
    cout << "B Grade\n";
} else if (grade >= 70) {
    cout << "C Grade\n";
} else {
    cout << "Failed\n";
}
```

### Nested If Statements
```cpp
bool hasTicket = true;
int age = 15;

if (hasTicket) {
    if (age >= 18) {
        cout << "Welcome to the movie!\n";
    } else {
        cout << "Need adult supervision\n";
    }
} else {
    cout << "Please buy a ticket\n";
}
```

### Switch Statement
```cpp
char grade = 'B';

switch (grade) {
    case 'A':
        cout << "Excellent!\n";
        break;
    case 'B':
        cout << "Good job!\n";
        break;
    case 'C':
        cout << "Fair\n";
        break;
    case 'F':
        cout << "Failed\n";
        break;
    default:
        cout << "Invalid grade\n";
}
```

### Switch with Multiple Cases
```cpp
int day = 3;

switch (day) {
    case 1:
    case 2:
    case 3:
    case 4:
    case 5:
        cout << "Weekday\n";
        break;
    case 6:
    case 7:
        cout << "Weekend\n";
        break;
    default:
        cout << "Invalid day\n";
}
```

### Ternary Operator
```cpp
int age = 20;
string status = (age >= 18) ? "Adult" : "Minor";
```

## 🎯 Condition Practice Problems

### Problem 1: Number Classifier
```cpp
int number;
cout << "Enter a number: ";
cin >> number;

if (number > 0) {
    cout << "Positive\n";
} else if (number < 0) {
    cout << "Negative\n";
} else {
    cout << "Zero\n";
}
```

### Problem 2: Grade Calculator
```cpp
int score;
cout << "Enter score (0-100): ";
cin >> score;

char grade;
if (score >= 90) grade = 'A';
else if (score >= 80) grade = 'B';
else if (score >= 70) grade = 'C';
else if (score >= 60) grade = 'D';
else grade = 'F';

cout << "Grade: " << grade << "\n";
```

## 📌 Conditional Statement Tips

1. 💡 Always use brackets {} even for single-line conditions
2. 💡 Consider all possible cases in switch statements
3. 💡 Don't forget break statements in switch cases
4. 💡 Use switch instead of if-else chains for multiple exact matches
5. 💡 Consider using ternary operator for simple conditions

## 🔍 Common Conditional Mistakes

1. Using = instead of == for comparison
2. Forgetting break statements in switch
3. Not handling all possible cases
4. Complex nested conditions (consider breaking into functions)
```
