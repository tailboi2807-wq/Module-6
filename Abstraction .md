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
~~~
from abc import ABC, abstractmethod

class Shape(ABC):
    @abstractmethod
    def calculate_area(self):
        pass

class Rectangle(Shape):
    def calculate_area(self):
        return 5 * 4

class Circle(Shape):
    def calculate_area(self):
        return 3.14 * 7 * 7

r = Rectangle()
c = Circle()

print("Rectangle Area:", r.calculate_area())
print("Circle Area:", c.calculate_area())
~~~
## Output
<img width="566" height="181" alt="image" src="https://github.com/user-attachments/assets/b3f9b12c-caa5-4d42-b52d-d948b1fc492e" />

## Result
The abstract method calculate_area() was successfully implemented in Rectangle and Circle, and their areas were calculated correctly.
