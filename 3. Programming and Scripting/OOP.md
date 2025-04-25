[L5DE M3T4.pdf](https://github.com/user-attachments/files/19906604/L5DE.M3T4.pdf)


🧠 Introduction to OOP
What is OOP?
A programming method that organizes code by bundling data (attributes) and functions (methods) into objects

Objects are like real-world components: they store data and do things

Communication between objects is key!

Why use OOP?
Models the real world 🌍

Keeps code clean + modular

Encapsulation protects data 🛡️

Makes complex systems manageable

🧱 Core Concepts
✅ Classes
Think of a class as a blueprint 🏗️

It defines properties (variables) + methods (functions)

✅ Objects
An object is an instance of a class

Like a real car from a "Car" class: it has its own color, speed, etc.

✅ Methods
Functions that belong to a class

They define what an object can do

✅ Properties / Attributes
Data stored in each object

Ex: name, salary, age

💻 Python Implementation
Defining a class
python
Copy
Edit
class Employee:
    def __init__(self, name, salary):
        self.name = name
        self.salary = salary
Instantiating objects
python
Copy
Edit
emp1 = Employee("Alice", 50000)
Setters & Validation
Can use methods like set_salary() to validate data before setting it.

🧠 Knowledge Check 💡
Q: What is a class?
A: B – A class defines the structure and behaviour of objects (blueprint!).

📦 Static Members
Static properties
Shared across all instances

Ex: min_salary, max_salary

Static methods
Don’t depend on instance data

python
Copy
Edit
@staticmethod
def is_valid_salary(salary):
    return salary >= 30000
🚀 Advanced OOP Concepts
🧵 Dataclass Decorators
Auto-generates __init__, __repr__, etc.

Clean, reduces boilerplate

python
Copy
Edit
from dataclasses import dataclass

@dataclass
class Person:
    name: str
    age: int
🧬 Polymorphism
Use different classes interchangeably

One interface, multiple forms 🧑‍🎓🧑‍🏫

🧬 Inheritance
A subclass inherits from a superclass

Promotes code reuse + hierarchy

python
Copy
Edit
class Manager(Employee):
    pass
🛡️ Encapsulation
Hides data using private variables

Provides controlled access via getters/setters
