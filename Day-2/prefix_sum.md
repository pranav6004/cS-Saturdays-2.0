### 3. Prefix Sum
The **Prefix Sum** algorithm precomputes cumulative sums of elements in an array, enabling efficient range sum queries. It is a powerful tool for problems involving cumulative data or range calculations.

#### Significance:
- Simplifies range query problems by reducing time complexity.
- Enables quick solutions for problems involving cumulative sums or differences.
- Forms the basis for more advanced algorithms like difference arrays or Fenwick trees.

## Pseudocode  
### Problem: Precompute prefix sums and query the sum of elements in a range `[l, r]`.  
```text
function prefix_sum(arr, queries):
    n ← length(arr)
    prefix ← array of size (n + 1) initialized to 0
    for i from 0 to n-1 do:
        prefix[i + 1] ← prefix[i] + arr[i]
    results ← empty list
    for (l, r) in queries do:
        results.append(prefix[r + 1] - prefix[l])
    return results
```

## Practice Problems
- [Range Sum Query - Immutable (LeetCode)](https://leetcode.com/problems/range-sum-query-immutable/)  
- [Subarray Sum Equals K (LeetCode)](https://leetcode.com/problems/subarray-sum-equals-k/)  
- [Sum of all subarrays (GeeksforGeeks)](https://www.geeksforgeeks.org/sum-of-all-subarrays/)
