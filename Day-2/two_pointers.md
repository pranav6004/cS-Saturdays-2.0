
### **1. Two Pointers**
The **Two Pointers** algorithm is a technique where two pointers are used to traverse a data structure in a specific way. It is often used to solve problems involving arrays or strings, such as finding pairs with a specific condition, merging arrays, or detecting overlapping intervals.

#### **Significance**:
- Simplifies problems involving sorted arrays or lists.
- Reduces time complexity compared to brute-force solutions.
- Commonly used in problems involving pairs, triplets, or sliding ranges.

## Pseudocode  
### Problem: Find a pair with a given sum in a sorted array.  
```text
function two_pointers(arr, target):
    left ← 0
    right ← length(arr) - 1
    while left < right do:
        current_sum ← arr[left] + arr[right]
        if current_sum = target then:
            return (left, right)
        else if current_sum < target then:
            left ← left + 1
        else:
            right ← right - 1
    return null

```

## Practice Problems
- [Two Sum II - Input Array Is Sorted (LeetCode)](https://leetcode.com/problems/two-sum-ii-input-array-is-sorted/)  
- [3Sum (LeetCode)](https://leetcode.com/problems/3sum/)  
- [Remove Duplicates from Sorted Array (LeetCode)](https://leetcode.com/problems/remove-duplicates-from-sorted-array/)