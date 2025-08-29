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
from abc import ABC, abstractmethod

class Shape(ABC): 
    @abstractmethod
    def area(self):    
        pass


class Rectangle(Shape):
    def __init__(self, length, breadth):
        self.__length = length      # private
        self.__breadth = breadth    # private

    def area(self):
        return self.__length * self.__breadth


class Circle(Shape):
    def __init__(self, radius):
        self.__radius = radius   # private

    def area(self):
        return 3.14 * self.__radius * self.__radius



r = Rectangle(6, 4)
c = Circle(7)


print("Area of a rectangle:", r.area())
print("Area of a circle:", c.area())

```
## Output

## Result
Thus the program is executed successfully.
