
### **2. Sliding Window**
The **Sliding Window** technique involves creating a window over a subset of data (like a subarray or substring) and moving it across the data structure. This technique is widely used in problems where you need to find optimal or feasible subarrays/substrings.

#### **Significance**:
- Optimizes brute-force approaches by reducing redundant calculations.
- Ideal for problems involving contiguous subarrays or substrings.
- Commonly used for problems like finding maximum/minimum sums, distinct elements, or satisfying conditions within a range.

## Pseudocode  
### Problem: Find the maximum sum of a subarray of size `k`.  
```text
function sliding_window(arr, k):
    n ← length(arr)
    if n < k then:
        return null
    window_sum ← 0
    for i from 0 to k-1 do:
        window_sum ← window_sum + arr[i]
    max_sum ← window_sum
    for i from k to n-1 do:
        window_sum ← window_sum + arr[i] - arr[i - k]
        max_sum ← max(max_sum, window_sum)
    return max_sum
```

## Practice Problems
- [Maximum Sum Subarray of Size K (GeeksforGeeks)](https://practice.geeksforgeeks.org/problems/max-sum-subarray-of-size-k5313/1)  
- [Longest Substring Without Repeating Characters (LeetCode)](https://leetcode.com/problems/longest-substring-without-repeating-characters/)  
- [Minimum Size Subarray Sum (LeetCode)](https://leetcode.com/problems/minimum-size-subarray-sum/)
