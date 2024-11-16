# Operators in Python

## Arithmetic Operators
```python
a = 10
b = 5

print(a + b)  # Addition: 15
print(a - b)  # Subtraction: 5
print(a * b)  # Multiplication: 50
print(a / b)  # Division: 2.0
print(a % b)  # Modulus: 0
print(a ** b) # Exponentiation: 100000
print(a // b) # Floor Division: 2
```

## Comparison Operators
```python
a = 10
b = 5

print(a == b)  # Equal: False
print(a != b)  # Not equal: True
print(a > b)   # Greater than: True
print(a < b)   # Less than: False
print(a >= b)  # Greater than or equal to: True
print(a <= b)  # Less than or equal to: False
```

## Logical Operators
```python
a = True
b = False

print(a and b) # Logical AND: False
print(a or b)  # Logical OR: True
print(not a)   # Logical NOT: False
```

## Bitwise Operators
```python
a = 10  # 1010 in binary
b = 4   # 0100 in binary

print(a & b)  # Bitwise AND: 0 (0000)
print(a | b)  # Bitwise OR: 14 (1110)
print(a ^ b)  # Bitwise XOR: 14 (1110)
print(~a)     # Bitwise NOT: -11 (inverts all bits)
print(a << 2) # Bitwise left shift: 40 (101000)
print(a >> 2) # Bitwise right shift: 2 (0010)
```

## Assignment Operators
```python
a = 10

a += 5  # a = a + 5
print(a) # 15

a -= 3  # a = a - 3
print(a) # 12

a *= 2  # a = a * 2
print(a) # 24

a /= 4  # a = a / 4
print(a) # 6.0

a %= 3  # a = a % 3
print(a) # 0.0

a **= 2 # a = a ** 2
print(a) # 0.0

a //= 2 # a = a // 2
print(a) # 0.0
```

## Membership Operators
```python
a = [1, 2, 3, 4, 5]

print(3 in a)  # True
print(6 in a)  # False
print(6 not in a) # True
```

## Identity Operators
```python
a = 10
b = 10

print(a is b)  # True
print(a is not b)  # False

c = [1, 2, 3]
d = [1, 2, 3]

print(c is d)  # False
print(c is not d)  # True
```