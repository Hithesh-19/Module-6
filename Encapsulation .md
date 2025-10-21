# 🐍 Python OOP: Encapsulation with Private Members

## 🎯 AIM

To implement **Encapsulation** in Python by defining a class `Rectangle` with **private member variables** `__length` and `__breadth`.

---

## 🧠 ALGORITHM

1. **Define the Class**:
   - Create a class `Rectangle` with two private attributes: `__length` and `__breadth`.

2. **Initialize Variables**:
   - Use the `__init__()` constructor to set initial values for `__length` and `__breadth`.

3. **Print Values**:
   - Display the private variables from within the class to demonstrate access.

4. **Instantiate the Object**:
   - Create an object of the `Rectangle` class to trigger the constructor.

---

## 💻 Program
```
class Rectangle:
    
    def __init__(self, length, breadth):
       
        self.__length = length  
        self.__breadth = breadth
    
        self.display_dimensions()
        print("----------------------")

    def display_dimensions(self):
        """Method to access and display the private attributes within the class."""
        print(f"Rectangle Length: {self.__length}")
        print(f"Rectangle Breadth: {self.__breadth}")
rectangle1 = Rectangle(length=15.0, breadth=5.5)
```
## Output
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/05bef73b-2042-4f1f-bc0a-016de90c17cd" />

## Result
Thus the program executed successfully.
