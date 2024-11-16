# Data Types in Python

Python supports various data types, each serving a different purpose. Here are some of the most commonly used data types:

## Numeric Types
1. **int**: Integer values
    ```python
    age = 25
    ```
2. **float**: Floating-point values
    ```python
    price = 19.99
    ```
3. **complex**: Complex numbers
    ```python
    complex_num = 1 + 2j
    ```

## Sequence Types
1. **str**: String values
    ```python
    name = "John"
    ```
2. **list**: Ordered, mutable collection
    ```python
    fruits = ["apple", "banana", "cherry"]
    ```
3. **tuple**: Ordered, immutable collection
    ```python
    coordinates = (10.0, 20.0)
    ```

## Mapping Type
1. **dict**: Key-value pairs
    ```python
    person = {"name": "Alice", "age": 30}
    ```

## Set Types
1. **set**: Unordered collection of unique elements
    ```python
    unique_numbers = {1, 2, 3, 4}
    ```
2. **frozenset**: Immutable version of a set
    ```python
    frozen_set = frozenset([1, 2, 3, 4])
    ```

## Boolean Type
1. **bool**: Boolean values
    ```python
    is_active = True
    ```

## None Type
1. **NoneType**: Represents the absence of a value
    ```python
    result = None
    ```

These data types form the foundation of Python programming and are essential for writing efficient and effective code.

## Common Methods and Properties

### List Methods
- **append()**: Adds an element to the end of the list
    ```python
    fruits.append("orange")
    ```
- **remove()**: Removes the first occurrence of an element
    ```python
    fruits.remove("banana")
    ```
- **pop()**: Removes and returns the element at the given index
    ```python
    fruits.pop(1)
    ```
- **sort()**: Sorts the list in ascending order
    ```python
    fruits.sort()
    ```
- **reverse()**: Reverses the elements of the list
    ```python
    fruits.reverse()
    ```

### Set Methods
- **add()**: Adds an element to the set
    ```python
    unique_numbers.add(5)
    ```
- **remove()**: Removes an element from the set
    ```python
    unique_numbers.remove(3)
    ```
- **union()**: Returns the union of sets
    ```python
    set1 = {1, 2, 3}
    set2 = {3, 4, 5}
    set3 = set1.union(set2)
    ```
- **intersection()**: Returns the intersection of sets
    ```python
    set3 = set1.intersection(set2)
    ```
- **difference()**: Returns the difference of sets
    ```python
    set3 = set1.difference(set2)
    ```

### Dictionary Methods
- **keys()**: Returns a view object of the dictionary's keys
    ```python
    keys = person.keys()
    ```
- **values()**: Returns a view object of the dictionary's values
    ```python
    values = person.values()
    ```
- **items()**: Returns a view object of the dictionary's key-value pairs
    ```python
    items = person.items()
    ```
- **get()**: Returns the value for the specified key
    ```python
    age = person.get("age")
    ```
- **update()**: Updates the dictionary with the specified key-value pairs
    ```python
    person.update({"city": "New York"})
    ```

### String Methods
- **upper()**: Converts a string to uppercase
    ```python
    name_upper = name.upper()
    ```
- **lower()**: Converts a string to lowercase
    ```python
    name_lower = name.lower()
    ```
- **find()**: Returns the index of the first occurrence of a substring
    ```python
    index = name.find("o")
    ```
- **replace()**: Replaces a substring with another substring
    ```python
    new_name = name.replace("John", "Jane")
    ```
- **split()**: Splits a string into a list of substrings
    ```python
    words = name.split()
    ```

These methods and properties are commonly used and can help you manipulate and interact with these data types effectively.