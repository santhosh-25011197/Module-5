# # Constructors in Python: Welcome Message with Student Name

## 🎯 Aim
To write a Python program that creates a **Student** class with a **default constructor** and a method to display a welcome message along with the student’s name provided by the user.

## 🧠 Algorithm
1. **Get user input**: Accept the student's name from the user.
2. **Define the class**: Create a class `Student` with a default constructor (`__init__`).
3. **Default Constructor**: In the constructor, assign the user input (student name) to an instance variable `self.a`.
4. **Display Message**: Define a method `show` that prints "This is non-parameterized constructor" and a welcome message with the student’s name.
5. **Execute the Program**: Instantiate the `Student` class and call the `show` method.

## 🧾 Program
```
class Student:
    def __init__(self):
        self.a = input("Enter student name: ")
    def show(self):
        print("This is non-parameterized constructor")
        print("Welcome", self.a)

obj = Student()
obj.show()
Add code here
```
## Output

<img width="406" height="276" alt="Screenshot 2026-03-25 210906" src="https://github.com/user-attachments/assets/d284a1fd-a9bd-45cb-97c0-be8c42ef0d94" />

## Result

Thus,the program was implemented and executed successfully,and the required output was obtained.

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


