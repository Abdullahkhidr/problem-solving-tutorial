# 📊 Arrays & Operations

## 📝 Array Basics

### Array Declaration
```cpp
// Fixed-size array declaration
int numbers[5];                    // Uninitialized array of 5 integers
int scores[5] = {90, 85, 88, 92, 95};  // Initialized array
int values[] = {1, 2, 3, 4, 5};   // Size automatically determined

// Common array types
char letters[26];                  // Character array
double prices[100];               // Double array
bool flags[10];                   // Boolean array
```

### Array Initialization Methods
```cpp
// Method 1: Initialize at declaration
int arr1[5] = {1, 2, 3, 4, 5};

// Method 2: Initialize with fewer elements (rest are 0)
int arr2[5] = {1, 2, 3};  // becomes {1, 2, 3, 0, 0}

// Method 3: Initialize all elements to 0
int arr3[5] = {0};

// Method 4: Initialize element by element
int arr4[5];
for(int i = 0; i < 5; i++) {
    arr4[i] = i * 2;  // {0, 2, 4, 6, 8}
}
```

## 🔄 Array Operations

### Accessing Elements
```cpp
int numbers[5] = {10, 20, 30, 40, 50};

// Using index
int firstElement = numbers[0];     // 10
int lastElement = numbers[4];      // 50

// Common mistake: accessing out of bounds
// numbers[5];  // Error! Valid indices are 0-4
```

### Modifying Elements
```cpp
int scores[3] = {75, 80, 85};

// Changing individual elements
scores[0] = 95;                    // Update first element
scores[2] += 5;                    // Increment last element

// After modifications: {95, 80, 90}
```

### Array Size
```cpp
// Getting array size
int numbers[] = {1, 2, 3, 4, 5};
int size = sizeof(numbers) / sizeof(numbers[0]);

cout << "Array size: " << size << "\n";  // Prints: 5
```

## 🔄 Array Traversal

### Using For Loop
```cpp
int arr[] = {10, 20, 30, 40, 50};
int size = sizeof(arr) / sizeof(arr[0]);

// Forward traversal
for(int i = 0; i < size; i++) {
    cout << arr[i] << " ";  // 10 20 30 40 50
}

// Backward traversal
for(int i = size - 1; i >= 0; i--) {
    cout << arr[i] << " ";  // 50 40 30 20 10
}
```

### Using Range-based For Loop
```cpp
int numbers[] = {1, 2, 3, 4, 5};

// Simple traversal
for(int num : numbers) {
    cout << num << " ";
}

// Using reference to modify elements
for(int &num : numbers) {
    num *= 2;  // Doubles each element
}
```

## 📊 Multi-dimensional Arrays

### 2D Arrays
```cpp
// Declaration and initialization
int matrix[3][3] = {
    {1, 2, 3},
    {4, 5, 6},
    {7, 8, 9}
};

// Accessing elements
int element = matrix[1][2];  // Gets 6

// Traversing 2D array
for(int i = 0; i < 3; i++) {
    for(int j = 0; j < 3; j++) {
        cout << matrix[i][j] << " ";
    }
    cout << "\n";
}
```

## 🎯 Common Array Operations

### Finding Maximum/Minimum
```cpp
int arr[] = {64, 34, 25, 12, 22, 11, 90};
int size = sizeof(arr) / sizeof(arr[0]);

int max_element = arr[0];
int min_element = arr[0];

for(int i = 1; i < size; i++) {
    if(arr[i] > max_element) {
        max_element = arr[i];
    }
    if(arr[i] < min_element) {
        min_element = arr[i];
    }
}
```

### Array Sum and Average
```cpp
int numbers[] = {10, 20, 30, 40, 50};
int size = sizeof(numbers) / sizeof(numbers[0]);

int sum = 0;
for(int num : numbers) {
    sum += num;
}

double average = static_cast<double>(sum) / size;
```

### Array Reversal
```cpp
void reverseArray(int arr[], int size) {
    for(int i = 0; i < size/2; i++) {
        // Swap elements
        int temp = arr[i];
        arr[i] = arr[size-1-i];
        arr[size-1-i] = temp;
    }
}
```

## 📌 Array Tips & Best Practices

1. 💡 Always check array bounds before accessing elements
2. 💡 Initialize arrays when declared if possible
3. 💡 Use appropriate data types for array elements
4. 💡 Consider using vectors for dynamic sizing
5. 💡 Be careful with array indexing (zero-based)

## 🚫 Common Array Mistakes

1. Array index out of bounds
2. Forgetting array size limits
3. Not initializing array elements
4. Incorrect array traversal bounds
5. Memory leaks with dynamic arrays

## 🔍 Debugging Tips

1. Print array elements to verify contents
2. Check array bounds in loops
3. Verify array initialization
4. Use debugger to watch array modifications
5. Test with different array sizes
```
