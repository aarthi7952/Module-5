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
