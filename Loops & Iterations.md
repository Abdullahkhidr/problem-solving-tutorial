# 🔄 Loops & Iterations

### For Loop
```cpp
// Basic for loop
for (int i = 0; i < 5; i++) {
    cout << i << " ";  // Prints: 0 1 2 3 4
}

// For loop with different step
for (int i = 0; i <= 10; i += 2) {
    cout << i << " ";  // Prints: 0 2 4 6 8 10
}

// Reverse for loop
for (int i = 5; i > 0; i--) {
    cout << i << " ";  // Prints: 5 4 3 2 1
}
```

### While Loop
```cpp
int count = 0;
while (count < 5) {
    cout << count << " ";
    count++;
}  // Prints: 0 1 2 3 4
```

### Do-While Loop
```cpp
int num = 1;
do {
    cout << num << " ";
    num *= 2;
} while (num <= 16);  // Prints: 1 2 4 8 16
```

### Nested Loops
```cpp
// Printing a multiplication table
for (int i = 1; i <= 3; i++) {
    for (int j = 1; j <= 3; j++) {
        cout << i << "x" << j << "=" << (i*j) << "\t";
    }
    cout << "\n";
}
/* Output:
1x1=1   1x2=2   1x3=3
2x1=2   2x2=4   2x3=6
3x1=3   3x2=6   3x3=9
*/
```

## 🎮 Loop Control Statements

### Break Statement
```cpp
// Exit loop when i equals 3
for (int i = 0; i < 5; i++) {
    if (i == 3) {
        break;
    }
    cout << i << " ";
}  // Prints: 0 1 2
```

### Continue Statement
```cpp
// Skip printing when i equals 2
for (int i = 0; i < 5; i++) {
    if (i == 2) {
        continue;
    }
    cout << i << " ";
}  // Prints: 0 1 3 4
```

### Infinite Loops
```cpp
// Infinite while loop
while (true) {
    cout << "This will run forever unless broken\n";
    // Use break condition to exit
    if (someCondition) break;
}

// Infinite for loop
for (;;) {
    cout << "This will also run forever\n";
    // Use break condition to exit
    if (someCondition) break;
}
```

## 🎯 Loop Practice Problems

### Problem 1: Sum of Numbers
```cpp
int sum = 0;
for (int i = 1; i <= 100; i++) {
    sum += i;
}
cout << "Sum of numbers 1-100: " << sum << "\n";
```

### Problem 2: Factorial Calculator
```cpp
int n;
cout << "Enter a number: ";
cin >> n;

long long factorial = 1;
for (int i = 1; i <= n; i++) {
    factorial *= i;
}
cout << n << "! = " << factorial << "\n";
```

### Problem 3: Pattern Printing
```cpp
int rows = 5;
for (int i = 1; i <= rows; i++) {
    for (int j = 1; j <= i; j++) {
        cout << "* ";
    }
    cout << "\n";
}
/* Output:
*
* *
* * *
* * * *
* * * * *
*/
```

## 🔄 Common Loop Patterns

### Array Traversal
```cpp
int arr[] = {1, 2, 3, 4, 5};
int size = sizeof(arr) / sizeof(arr[0]);

for (int i = 0; i < size; i++) {
    cout << arr[i] << " ";
}

// Range-based for loop (C++11 and later)
for (int num : arr) {
    cout << num << " ";
}
```

### String Processing
```cpp
string text = "Hello";
for (char c : text) {
    cout << c << " ";
}  // Prints: H e l l o
```

## 📌 Loop Tips & Best Practices

1. 💡 Always check loop conditions to avoid infinite loops
2. 💡 Use appropriate loop type for your needs:
   - For loop: When number of iterations is known
   - While loop: When condition-based iteration is needed
   - Do-while: When you need at least one iteration
3. 💡 Be careful with loop variables:
   - Initialize properly
   - Update correctly
   - Check boundary conditions
4. 💡 Consider performance with nested loops
5. 💡 Use break and continue wisely

## 🚫 Common Loop Mistakes

1. Off-by-one errors (incorrect loop bounds)
2. Forgetting to update loop variables
3. Infinite loops due to incorrect conditions
4. Unnecessary nested loops
5. Wrong loop type selection

## 🔍 Loop Debugging Tips

1. Print loop variables to track iterations
2. Check boundary conditions
3. Verify loop update statements
4. Test with different input sizes
5. Use debugger for step-by-step execution
```
