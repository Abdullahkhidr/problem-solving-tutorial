# 📝 Strings & String Operations

## 📌 String Basics

### String Declaration
```cpp
// Different ways to declare strings
string str1;                    // Empty string
string str2 = "Hello";         // Direct initialization
string str3("World");          // Constructor initialization
string str4 = str2 + " " + str3;  // "Hello World"

// C-style strings (char arrays)
char str5[] = "Hello";         // Null-terminated string
char str6[6] = {'H','e','l','l','o','\0'};
```

### String Input/Output
```cpp
string name;

// Single word input
cin >> name;

// Full line input
getline(cin, name);

// Output
cout << name << endl;
```

## 🔄 String Operations

### String Length and Capacity
```cpp
string text = "Hello World";
int length = text.length();     // or text.size()
int capacity = text.capacity(); // Allocated space
bool isEmpty = text.empty();    // Check if empty
```

### String Concatenation
```cpp
string first = "Hello";
string second = "World";

// Method 1: Using + operator
string result = first + " " + second;

// Method 2: Using append()
first.append(" ").append(second);

// Method 3: Using +=
first += " " + second;
```

### String Access and Modification
```cpp
string str = "Hello";

// Accessing characters
char first = str[0];           // 'H'
char last = str.back();        // 'o'

// Modifying characters
str[0] = 'h';                  // "hello"
str.at(1) = 'E';              // "hEllo"

// Substring
string sub = str.substr(1, 3); // "Ell"
```

## 🔍 String Searching

### Find Operations
```cpp
string text = "Hello World";

// Finding substrings
size_t pos = text.find("World");     // Returns 6
pos = text.find('o');                // Returns 4
pos = text.rfind('o');               // Returns 7 (last occurrence)

// Check if found
if (pos != string::npos) {
    cout << "Found at position: " << pos << "\n";
}
```

### Find and Replace
```cpp
string text = "Hello World";

// Replace first occurrence
text.replace(0, 5, "Hi");     // "Hi World"

// Replace all occurrences
size_t pos = 0;
while ((pos = text.find("l", pos)) != string::npos) {
    text.replace(pos, 1, "L");
    pos += 1;
}
```

## 🔄 String Manipulation

### Insert and Erase
```cpp
string str = "Hello";

// Insert
str.insert(5, " World");      // "Hello World"
str.insert(0, "Say ");        // "Say Hello World"

// Erase
str.erase(0, 4);              // "Hello World"
str.erase(5);                 // "Hello"
```

### Push and Pop Operations
```cpp
string str = "Hello";

// Add characters
str.push_back('!');           // "Hello!"
str.pop_back();               // "Hello"
```

## 📊 String Comparison

### Comparison Operations
```cpp
string str1 = "Hello";
string str2 = "World";

bool isEqual = (str1 == str2);         // false
bool isLess = (str1 < str2);           // true
bool isGreater = (str1 > str2);        // false

// Compare specific portions
int result = str1.compare(0, 2, str2, 0, 2);
```

## 🔄 String Transformation

### Case Conversion
```cpp
string text = "Hello World";

// Convert to upper/lower case
for(char &c : text) {
    c = toupper(c);           // "HELLO WORLD"
}

for(char &c : text) {
    c = tolower(c);           // "hello world"
}
```

## 🎯 String Practice Problems

### Problem 1: Reverse String
```cpp
string str;
cin >> str;
int n = str.length();
for(int i = 0; i < n/2; i++) {
    swap(str[i], str[n-1-i]);
}
cout << str;
```
## 📌 String Best Practices

1. 💡 Use string class over C-style strings when possible
2. 💡 Check string bounds before accessing characters
3. 💡 Use appropriate string functions for operations
4. 💡 Consider string capacity for performance
5. 💡 Handle empty strings appropriately

## 🚫 Common String Mistakes

1. Forgetting to check string::npos when searching
2. Not handling empty strings
3. Array index out of bounds
4. Incorrect substring parameters
5. Memory leaks with C-style strings

## 🔍 String Debugging Tips

1. Print string length and content
2. Check string bounds in operations
3. Verify string modifications
4. Test with empty strings
5. Test with special characters
```
