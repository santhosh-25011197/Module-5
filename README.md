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


# Hierarchical Inheritance in Python

This Python project demonstrates **Hierarchical Inheritance** using a base class `Details` and two derived classes `Employee` and `Patient`. The program collects and displays details for both employees and patients.

## 🎯 Aim

To write a Python program that uses **Hierarchical Inheritance** to input and display **Employee** and **Patient** details.

## 📘 Description

- **Base Class:** `Details`
  - Stores common attributes: `name`, `age`
  - Provides methods: `getName()`, `getAge()`

- **Derived Class 1:** `Employee`
  - Inherits from `Details`
  - Adds: `employee_id`, `department`
  - Method: `getEmployeeDetails()`

- **Derived Class 2:** `Patient`
  - Inherits from `Details`
  - Adds: `patient_id`, `disease`
  - Method: `getPatientDetails()`

## 🧠 Algorithm

1. Create base class `Details` with common attributes.
2. Create `Employee` class extending `Details`, adding employee-specific data.
3. Create `Patient` class extending `Details`, adding patient-specific data.
4. Get user input for employee and patient data.
5. Display collected information using class methods.

## Program
```
class Details:
    def getName(self):
        self.name = input("Enter name: ")
    def getAge(self):
        self.age = int(input("Enter age: "))


class Employee(Details):
    def getEmployeeDetails(self):
        self.employee_id = input("Enter employee id: ")
        self.department = input("Enter department: ")
        print("\nEmployee Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Employee ID:", self.employee_id)
        print("Department:", self.department)


class Patient(Details):
    def getPatientDetails(self):
        self.patient_id = input("Enter patient id: ")
        self.disease = input("Enter disease: ")
        print("\nPatient Details")
        print("Name:", self.name)
        print("Age:", self.age)
        print("Patient ID:", self.patient_id)
        print("Disease:", self.disease)


e = Employee()
e.getName()
e.getAge()
e.getEmployeeDetails()

p = Patient()
p.getName()
p.getAge()
p.getPatientDetails()
```
## Sample Output

<img width="294" height="388" alt="image" src="https://github.com/user-attachments/assets/7a78046f-c7cb-4e6e-bcbb-98f3b77c8f74" />

##  Result

Thus, the code was executed successfully.


# Multilevel Inheritance Example in Python

This Python project demonstrates the concept of **Multilevel Inheritance** to collect and display the **name**, **age**, and **location** of a person.

## 🎯 Aim

To write a Python program that uses multilevel inheritance to get and display a person’s name, age, and location.

## 🧠 Algorithm

1. **Parent Class**  
   - `__init__(name)` initializes the `name` attribute.  
   - `getName()` returns the `name`.

2. **Child Class (inherits Parent)**  
   - `__init__(name, age)` initializes `name` using `super()` and adds `age`.  
   - `getAge()` returns the `age`.

3. **Grandchild Class (inherits Child)**  
   - `__init__(name, age, location)` initializes `name` and `age` using `super()` and adds `location`.  
   - `getLocation()` returns the `location`.

4. **Input & Output**  
   - Take user input for name, age, and location.  
   - Create an instance of `Grandchild`.  
   - Print all details using class methods.

## Program
```
class Parent:
    def __init__(self, name):
        self.name = name

    def getName(self):
        return self.name


class Child(Parent):
    def __init__(self, name, age):
        super().__init__(name)
        self.age = age

    def getAge(self):
        return self.age


class Grandchild(Child):
    def __init__(self, name, age, location):
        super().__init__(name, age)
        self.location = location

    def getLocation(self):
        return self.location


name = input("Enter name: ")
age = int(input("Enter age: "))
location = input("Enter location: ")

obj = Grandchild(name, age, location)

print("Name:", obj.getName())
print("Age:", obj.getAge())
print("Location:", obj.getLocation())
```
## Sample Output

<img width="375" height="325" alt="image" src="https://github.com/user-attachments/assets/5eebfa62-a7dd-4898-9bd7-891c374a1c44" />

## Result

Thus, the code was successfully executed.


