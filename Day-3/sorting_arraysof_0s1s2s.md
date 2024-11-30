## Sort an array of 0s, 1s and 2s – Dutch National Flag Problem

The Dutch National Flag Problem is a classic computer science problem introduced by Edsger Dijkstra. The problem involves sorting an array of elements into three categories or groups: typically, these elements are represented by the numbers 0, 1, and 2, and the goal is to sort the array such that all 0s are at the beginning, all 1s are in the middle, and all 2s are at the end.

## Problem Statement:
Given an array containing only 0s, 1s, and 2s, sort the array such that:

1. All 0s appear first.
2. All 1s appear second.
3. All 2s appear last.

## Pseudo Code
``` text
sort012(vector<int> &arr) {
    int n = arr.size();
    int c0 = 0, c1 = 0, c2 = 0;

    // Count 0s, 1s and 2s
    for (int i = 0; i < n; i++) {
        if (arr[i] == 0)
            c0 += 1;
        else if (arr[i] == 1)
            c1 += 1;
        else
            c2 += 1;
    }

    int idx = 0;
    
    // Place all the 0s
    for (int i = 0; i < c0; i++)
        arr[idx++] = 0;

    // Place all the 1s
    for (int i = 0; i < c1; i++)
        arr[idx++] = 1;

    // Place all the 2s
    for (int i = 0; i < c2; i++)
        arr[idx++] = 2;
}
```

## Time Complexity

- **Time Complexity**: O(n), where n is the number of elements in the array. We iterate over the array three times (once for counting, and twice for placing values).
- **Space Complexity**: O(1), as we are only using a few counters (c0, c1, c2) and an index pointer, which are independent of the size of the array.

## Practice Problems
- [Sort 0s, 1s, 2s - GeeksforGeeks](https://www.geeksforgeeks.org/problems/sort-an-array-of-0s-1s-and-2s4231/1)
- [Sort Colors - LeetCode](https://leetcode.com/problems/sort-colors/description/)
- [Segregate 0s and 1s - GeeksforGeeks](https://www.geeksforgeeks.org/problems/segregate-0s-and-1s5106/1?itm_source=geeksforgeeks&itm_medium=article&itm_campaign=practice_card)