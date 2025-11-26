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
class student:
    def __init__(self):
        print("This is non parametrized constructor")
    def display_welcome(self,name):
        print(f"Hello {name}")
name=input()
studentinstance=student()
studentinstance.display_welcome(name)
```
## Output
<img width="838" height="220" alt="517439870-1e27d533-20b2-446d-918a-066f0218b016" src="https://github.com/user-attachments/assets/64f7cc54-2b03-46e5-84ab-83d63a62798a" />

## Result
Thus the output is Verified.
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
        print ("Alive")
    def __del__(self):
        print("The object no longer exists")
obj=Demo()
```

## 🧪 Output
<img width="595" height="163" alt="517440436-da1908e7-9f57-4051-bcda-aa05a6b10c04" src="https://github.com/user-attachments/assets/c5f0e328-0511-4ee8-a90f-cf239c19f018" />

## Result
Thus the output is verified.
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
# Single inheritance in python
#Base class
class Details(object): 
# Constructor 
    def __init__(self, name, id): 
        self.name = name 
        self.id = id
# To fetch employee details 
    def Employee_Details(self): 
        return self.id , self.name
# derived class or the sub class
class Patient_details(Employee_details): 
    # To check if this  is a valid employee 
    def Employee_check(self): 
        if self.id > 500000:
           return " Valid Employee "
        else:
           return " Invalid Employee "
# Driver code 
id=int(input())
name=input()
Employee1 = Patient_details( name , id)  # parent class object
print( Employee1.Employee_Details() , Employee1.Employee_check() )
```
## Sample Output
<img width="811" height="229" alt="517440870-ea01142f-03a2-4a59-8e95-a6549b12702c" src="https://github.com/user-attachments/assets/013bc8f0-0317-47d3-a0df-786aa22868df" />
## Result
Thus the output is verified.

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
   def __init__(self,name):
     self.name = name
   def getName(self):
     return self.name
class Child(Parent):
   def __init__(self,name,age):
     Parent.__init__(self,name)
     self.age = age
   def getAge(self):
     return self.age
class Grandchild(Child):
   def __init__(self,name,age,location):
     Child.__init__(self,name,age)
     self.location=location
   def getLocation(self):
     return self.location
name=input()
age=int(input())
loc=input()
gc = Grandchild(name,age,loc)
print(gc.getName(), gc.getAge(), gc.getLocation())
```

## Sample Output
<img width="584" height="181" alt="486530944-f59e1195-c99d-4bed-82b6-f0c472869288" src="https://github.com/user-attachments/assets/40463465-cd6c-467d-9e17-7be9aecb8248" />

## Result
The code is verified successfully.
# Arithmetic Operations Using Multiple Inheritance in Python

This Python program demonstrates **multiple inheritance** by performing basic arithmetic operations — Addition, Subtraction, and Division — using three classes.

## 🎯 Aim

To write a Python program to calculate **Add, Sub & Division** using **Multiple Inheritance**.

## 🧠 Algorithm

1. **Define `Calculation1` class**
   - Contains `Summation(a, b)` method to return the sum of two numbers.
2. **Define `Calculation2` class**
   - Contains `Subtraction(a, b)` method to return the difference of two numbers.
3. **Define `Derived` class**
   - Inherits from both `Calculation1` and `Calculation2`.
   - Contains `Division(a, b)` method to return the division result.
4. **Input**
   - Prompt the user to enter two numbers.
5. **Process**
   - Create an object of the `Derived` class.
   - Call `Summation`, `Subtraction`, and `Division` methods.
6. **Output**
   - Display the results of the three operations.

## 💻 Program 
```
class Calculation1:  
    def Summation(self,a,b):  
        return a+b;  
class Calculation2:  
    def sub(self,a,b):  
        return a-b;  
class Derived(Calculation1,Calculation2):  
    def Mul(self,a,b):  
        return a*b;  
a=int(input())
b=int(input())
d = Derived()  
print(d.Summation(a,b))  
print(d.sub(a,b))  
print(d.Mul(a,b))
```
## Output Example
<img width="334" height="209" alt="486531164-33a0230d-71ef-43a9-83db-de167871c1bf" src="https://github.com/user-attachments/assets/396aa3d0-e1e4-4287-aa15-bb0b784a5b52" />

## Result
The multiple inheritence is verified successfully.


