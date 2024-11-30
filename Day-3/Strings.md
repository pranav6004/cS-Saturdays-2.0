## Strings
A string is simply a sequence of characters, such as letters, numbers, punctuation, or whitespace. These characters are usually stored and manipulated in programming languages. Strings can be as simple as a single letter or number, or they can be long sentences or paragraphs.
- "Hello"
- "12345"
- "Computer Science"
- "!@#"
- "" (An empty string)

#### In most programming languages, strings are enclosed in either double quotes (" ") or single quotes (' '), but this depends on the language.

## How Strings are Used in Programming
Strings are used to represent and manipulate textual data in programs. For example, they might store names, addresses, or other textual information. You can also perform various operations on strings, such as searching, comparing, or modifying them.

## Basic Operations on Strings
Here are some common operations you can perform on strings:

### **Concatenation**: Joining two or more strings together.
*Example*: "Hello " + "World" gives "Hello World"

### **Length**: Counting the number of characters in a string.
*Example*: "Hello".length() would return 5.

### Accessing Characters: You can access individual characters in a string using an index.
*Example*: "Hello"[0] would return 'H' (indexing starts from 0).

### Slicing: Extracting a portion of the string using start and end indices.
*Example*: "Hello"[1:4] would return "ell" (it starts at index 1 and ends just before index 4).

### String Comparison: Checking if two strings are equal.
*Example*: "Hello" == "Hello" would return True (or false if the strings are different).

### **Searching**: Finding the position of a substring in a string.
*Example*: "Hello".find("e") would return 1 (since "e" is at index 1 in "Hello").

## Reversal of a String:

### Pseudo Code
``` text
Function ReverseString(inputString):
    Initialize left pointer to 0
    Initialize right pointer to length of inputString - 1
    
    While left pointer < right pointer:
        // Swap characters at left and right pointers
        temp = inputString[left]
        inputString[left] = inputString[right]
        inputString[right] = temp
        
        // Move pointers towards the center
        left pointer = left pointer + 1
        right pointer = right pointer - 1
    
    Return inputString
```

## Practice Problems
- [Reverse of a String - LeetCode](https://leetcode.com/problems/reverse-string/)
- [Check if the string is Palindrome - GeeksforGeeks](https://www.geeksforgeeks.org/problems/palindrome-string0817/1)
- [Sort characters by frequency - LeetCode](https://leetcode.com/problems/sort-characters-by-frequency/description/)