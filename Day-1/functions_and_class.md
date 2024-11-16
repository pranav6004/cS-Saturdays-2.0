# Notes on Functions and Classes in Python

## Functions

### Definition
A function is a block of organized, reusable code that is used to perform a single, related action. Functions provide better modularity for your application and a high degree of code reusability.

### Syntax
```python
def function_name(parameters):
    """docstring"""
    statement(s)
```

### Example
```python
def greet(name):
    """This function greets the person passed in as a parameter"""
    print(f"Hello, {name}!")

greet('Alice')
```

### Key Points
- Functions help break our program into smaller and modular chunks.
- Function definitions begin with the `def` keyword.
- The parameters (arguments) are optional.
- The `return` statement is used to exit a function and go back to the place from where it was called.

## Classes

### Definition
A class is a blueprint for creating objects. Classes encapsulate data for the object and methods to manipulate that data.

### Syntax
```python
class ClassName:
    """docstring"""
    class_variable = 'value'

    def __init__(self, parameters):
        self.instance_variable = parameters

    def method(self):
        statement(s)
```

### Example
```python
class Dog:
    """A simple class to model a dog"""
    
    def __init__(self, name, age):
        self.name = name
        self.age = age

    def bark(self):
        print(f"{self.name} says woof!")

my_dog = Dog('Buddy', 3)
my_dog.bark()
```

### Key Points
- Classes provide a means of bundling data and functionality together.
- Creating a new class creates a new type of object, allowing new instances of that type to be made.
- The `__init__` method initializes the object's attributes.
- Methods are functions that belong to the class.
