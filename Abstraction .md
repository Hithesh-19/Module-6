# 🐍 Python OOP: Abstract Class & Method Example

## 🎯 AIM

To create an **abstract class** named `Shape` with an **abstract method** `calculate_area`, and implement this method in two subclasses: `Rectangle` and `Circle`.

---

## 🧠 ALGORITHM

1. **Import ABC module**:
   - Use `from abc import ABC, abstractmethod` to define abstract classes and methods.

2. **Create Abstract Class `Shape`**:
   - Define an abstract method `calculate_area()` with `@abstractmethod`.

3. **Create Subclass `Rectangle`**:
   - Set default values for `length` and `breadth`.
   - Override `calculate_area()` to compute the rectangle area.

4. **Create Subclass `Circle`**:
   - Set default value for `radius`.
   - Override `calculate_area()` to compute the circle area.

5. **Create Objects & Call Methods**:
   - Instantiate `Rectangle` and `Circle`.
   - Call their `calculate_area()` methods.

---

## 💻 Program
```
from abc import ABC, abstractmethod
import math


class Shape(ABC):
    
    @abstractmethod
    def calculate_area(self):
        
        pass

class Rectangle(Shape):
  

    def __init__(self, length=10, breadth=5):
        self.length = length
        self.breadth = breadth

    
    def calculate_area(self):
        """Computes the area of the rectangle (length * breadth)."""
        area = self.length * self.breadth
        return area
    
class Circle(Shape):
    """
    A concrete subclass of Shape for calculating the area of a circle.
    """
    

    def __init__(self, radius=7):
        self.radius = radius

    def calculate_area(self):
        """Computes the area of the circle (pi * radius^2)."""
        area = math.pi * (self.radius ** 2)
        return area


rectangle = Rectangle() 
rectangle_area = rectangle.calculate_area()


circle = Circle(radius=3) 
circle_area = circle.calculate_area()

print("---")
print("Area Calculations using Abstract Class Inheritance:")
print("---")

print(f"Rectangle (Length={rectangle.length}, Breadth={rectangle.breadth}):")
print(f"Area: {rectangle_area}")

print("\n---")


print(f"Circle (Radius={circle.radius}):")
print(f"Area: {circle_area:.2f}") 
```

## Output
<img width="1920" height="1080" alt="image" src="https://github.com/user-attachments/assets/e9117416-b8c0-4148-9c59-844f7fef3972" />


## Result
Thus the program executed successfully.
