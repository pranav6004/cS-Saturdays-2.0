# Time and Space Complexity

In Computer Science, there is more than one way of solving a problem. Hence, a universal method of measuring each solution is required. Time and Space complexity are used to judge how accurate and efficient your solution is. These are two fundamental metrics used to evaluate the performance of algorithms, especially in contexts like coding competitions or real-world applications where efficiency is crucial.

## What is Time Complexity?

When you write a program, you want to know how fast or slow it runs. Time complexity is a way to measure how the time your program takes grows as the size of the input grows. It's like asking: "If I give you more work to do (more data), how much longer will it take?"

## Why is Time Complexity important?

As your programs grow more complex or handle larger amounts of data, the time it takes to run your code can become really important. For example, if your program has to handle 10,000 numbers instead of just 10, you want to know if it will still run in a reasonable time.

**Time Complexity** measures the amount of time an algorithm takes to complete as a function of the size of the input. It gives us a way to evaluate how the runtime of an algorithm scales as the input size grows. 

#### Common time complexities include:
- Constant time (O(1)): The algorithm takes the same amount of time, no matter how large the input is.
- Logarithmic time (O(log n)): The time grows directly with the size of the input.
- Linear time (O(n)): The time grows much slower as the input size increases.
- Quadratic time (O(n^2)): The time grows with the square of the input size.

Let's look at a simple pseudo code example to calculate the time complexity of an operation that involves two numbers.

### Example 1: Addition of two numbers

#### Pseudo code  
```text
function addTwoNumbers(a, b):
    result = a + b  // Constant time operation
    return result
```
### Time Complexity Analysis

- The addition operation (a + b) is performed once.
- No matter how large a and b are, it takes a constant time to compute the sum.
- Time Complexity = O(1)
- Constant time.

### Example 2: Addition of two matrices

#### Pseudo code  
```text
function addMatrices(A, B):
    # Get the number of rows (m) and columns (n) from the matrices
    m = number of rows in A
    n = number of columns in A

    # Create a new matrix C to store the result, initialized to zero
    C = new matrix of size m x n

    # Loop through each element of the matrices
    for i = 1 to m:         # Iterate through rows
        for j = 1 to n:     # Iterate through columns
            C[i][j] = A[i][j] + B[i][j]  # Add corresponding elements

    return C  # Return the result matrix
```
### Time Complexity Analysis:
1. Loop Iterations:

- There are two nested loops in the pseudocode.
- The outer loop (over i) runs from 1 to m, meaning it runs m times (where m is the number of rows).
- The inner loop (over j) runs from 1 to n, meaning it runs n times (where n is the number of columns).
- Total Operations:

2. For each iteration of the outer loop, the inner loop runs n times.
- This gives a total of m * n iterations, as for each of the m rows, we perform n operations (adding corresponding elements of matrices A and B).
- Constant-time Operations inside the Loop:

3. The operation inside the inner loop (C[i][j] = A[i][j] + B[i][j]) is a constant-time operation. It just adds two numbers and assigns the result, which takes the same amount of time regardless of the size of the input.

**Time Complexity**: Since there are m * n iterations, and each iteration involves a constant-time operation, the overall time complexity of the algorithm is O(m * n). It falls under the category of *quadratic time complexity*.

## What is Space Complexity?
Space complexity is all about how much memory your program needs to run, depending on how big your input is.

It is mesure of the amount of memory (or space) an algorithm uses as a function of the size of the input.

When analyzing space complexity, we're interested in:

- Fixed memory (memory used for variables, constants, etc.),
- Dynamic memory (memory used for things like arrays, lists, or recursion stack), which can change depending on the input.

### Constant Space Complexity - O(1)
An algorithm with O(1) space complexity uses a constant amount of memory, regardless of the size of the input. This means the memory usage does not change even if the input size increases.

### Example 1: Finding the Maximum in a List

#### Pseudo code
``` text
function findMax(numbers):
    max_value = numbers[0]  # Use one variable to store the max value
    for num in numbers:     # Loop through the list
        if num > max_value:
            max_value = num
    return max_value
```
### Space Complexity Analysis:

- We are only using a single variable max_value to keep track of the largest number.
- The amount of memory used by this algorithm doesn't change with the size of the input list numbers.
- Space Complexity = O(1) (constant space).

### Linear Space Complexity - O(n)
An algorithm with O(n) space complexity uses memory that grows linearly with the input size. This usually happens when the algorithm creates a data structure like an array, list, or other collection that stores elements based on the input size.

### Example 2: Storing the Squares of Numbers
#### Pseudo code
``` text
function storeSquares(numbers):
    squares = []              # Create an empty list to store results
    for num in numbers:       # Loop through the list of numbers
        squares.append(num * num)  # Add the square of each number to the list
    return squares
```

### Space Complexity Analysis:

- We create a list squares to store the squares of the numbers. The size of this list depends on the size of the input list numbers.
- If there are n numbers in the input list, the squares list will also have n elements.
- Space Complexity = O(n) (linear space).




