# Destructor in Python

This project demonstrates how to implement a **destructor** in Python using a simple class.

## 🚀 Overview

The program defines a class `Demo` with:

- A **constructor** `__init__` that initializes an instance variable and prints a message.
- A **destructor** `__del__` that prints a message when the object is destroyed.

## 🧠 Algorithm

1. Define a class named `Demo`.
2. Inside the class, define the `__init__` method:
   - Initialize an instance variable `status` with the value `"Alive"`.
   - Print the value of `status`.
3. Define the `__del__` method:
   - Print a message indicating the object is being destroyed.
4. Outside the class:
   - Create an instance of the `Demo` class.
   - Delete the object using the `del` keyword.
## Program
```
class Demo:
    def __init__(self):
        self.status = "Alive"
        print(self.status)
    def __del__(self):
        print("Object is destroyed")

obj = Demo()
del obj
```

## 🧪 Output

<img width="375" height="266" alt="Screenshot 2026-03-25 211136" src="https://github.com/user-attachments/assets/88bdf839-da92-49b0-9443-805fd3da00d8" />


## Result
Thus, the code was completed and implemented successfully.


