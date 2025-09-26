
---

# Exception Handling in C++

## 📚 **Aim**

To understand **exception handling** in C++ using `try`, `catch`, and `throw`, and to implement:

* Program 1: Throw an exception if age < 18.
* Program 2: Basic exception handling demonstration.

## 🛠 **Tools**

* GNU g++ compiler for local compilation
* Any online C++ compiler

---

## 📝 **Theory**

**Exception handling** in C++ allows a program to handle **runtime errors** gracefully without crashing.
It uses three main keywords:

* **try** – The block of code to monitor for exceptions.
* **throw** – Used to signal (throw) an exception.
* **catch** – Handles the thrown exception.

Benefits:

* Improves program stability.
* Separates error handling from normal code.
* Prevents abrupt program termination.

---

## 💻 **Programs**

### **Program 1: Exception – Age Less Than 18**

**Logic:**
Checks if entered age is less than 18. If true, throws an exception; otherwise, displays eligibility message.

**Algorithm:**

1. Start.
2. Input `age`.
3. Use a `try` block to check if age < 18.
4. If yes, `throw` an exception.
5. Use a `catch` block to handle the exception and print an error message.
6. End.

**Sample Code:**

```cpp
#include <iostream>
using namespace std;

int main() {
    int age;
    cout << "Enter your age: ";
    cin >> age;

    try {
        if (age < 18)
            throw age; // throw exception
        else
            cout << "You are eligible." << endl;
    }
    catch (int ageValue) {
        cout << "Exception: Age " << ageValue << " is less than 18. Not eligible." << endl;
    }

    return 0;
}
```

---

### **Program 2: Basic Exception Handling**

**Logic:**
Demonstrates basic `try`, `catch`, `throw` for operations such as division by zero.

**Algorithm:**

1. Start.
2. Input two numbers.
3. Check denominator. If zero, `throw` an exception.
4. `catch` block handles division-by-zero error.
5. Else perform division.
6. End.

**Sample Code:**

```cpp
#include <iostream>
using namespace std;

int main() {
    int num, den;
    cout << "Enter numerator: ";
    cin >> num;
    cout << "Enter denominator: ";
    cin >> den;

    try {
        if (den == 0)
            throw den; // throw exception
        cout << "Result: " << (float)num / den << endl;
    }
    catch (int) {
        cout << "Exception: Division by zero is not allowed." << endl;
    }

    return 0;
}
```

---

## ✅ **Conclusion**

Exception handling in C++ helps manage errors safely without crashing the program.

* **Program 1** shows how to throw an exception if a condition (age < 18) is met.
* **Program 2** shows how to catch and handle a runtime error (division by zero).

Using `try`, `catch`, and `throw` ensures your program is **robust**, **secure**, and **user-friendly**.

---


