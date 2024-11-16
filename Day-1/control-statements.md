# Control Statements in Python

Control statements in Python are used to control the flow of execution of the program. Here are a few examples:

## If Statement

The `if` statement is used to test a condition. If the condition is true, the block of code inside the `if` statement is executed.

```python
x = 10
if x > 5:
    print("x is greater than 5")
```

## If-Else Statement

The `if-else` statement is used to test a condition and execute one block of code if the condition is true and another block of code if the condition is false.

```python
x = 10
if x > 5:
    print("x is greater than 5")
else:
    print("x is not greater than 5")
```

## Elif Statement

The `elif` statement is used to test multiple conditions. If the first condition is false, it checks the next condition, and so on.

```python
x = 10
if x > 15:
    print("x is greater than 15")
elif x > 5:
    print("x is greater than 5 but less than or equal to 15")
else:
    print("x is 5 or less")
```

### Problems On Conditionals
- [Python If-Else HackerRank](https://www.hackerrank.com/challenges/py-if-else/problem?isFullScreen=true)
- [Check The Status GFG](https://www.geeksforgeeks.org/problems/check-the-status/1?page=1&category=python&difficulty=Easy&sortBy=submissions)

## While Loop

The `while` loop is used to repeat a block of code as long as a condition is true.

```python
x = 0
while x < 5:
    print(x)
    x += 1
```

## For Loop

The `for` loop is used to iterate over a sequence (such as a list, tuple, or string) and execute a block of code for each item in the sequence.

```python
fruits = ["apple", "banana", "cherry"]
for fruit in fruits:
    print(fruit)
```

## Break Statement

The `break` statement is used to exit a loop prematurely.

```python
for i in range(10):
    if i == 5:
        break
    print(i)
```

## Continue Statement

The `continue` statement is used to skip the rest of the code inside a loop for the current iteration and continue with the next iteration.

```python
for i in range(10):
    if i % 2 == 0:
        continue
    print(i)
```

## Pass Statement

The `pass` statement is a null operation; it is used when a statement is required syntactically but no code needs to be executed.

```python
for i in range(10):
    if i % 2 == 0:
        pass
    else:
        print(i)
```

### Problems On Conditionals
- [Loops HackerRank](https://www.hackerrank.com/challenges/python-loops/problem?isFullScreen=true)
- [For Loop GFG](https://www.geeksforgeeks.org/problems/for-loop-python/1?page=1&category=python&sortBy=submissions)
- [While Loop GFG](https://www.geeksforgeeks.org/problems/while-loop-in-python/1?page=1&category=python&sortBy=submissions)


These are some of the basic control statements in Python that help in controlling the flow of the program.