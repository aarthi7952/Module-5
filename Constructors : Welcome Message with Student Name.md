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
