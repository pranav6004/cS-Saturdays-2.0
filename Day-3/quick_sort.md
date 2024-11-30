## Quick Sort Algorithm

Quick Sort is a divide-and-conquer algorithm for sorting a list or array. It works by selecting a "pivot" element and partitioning the array into two sub-arrays — one containing elements less than the pivot and one containing elements greater than the pivot. It then recursively sorts the sub-arrays.

## Steps of Quick Sort:

- **Pick a pivot**: Choose an element from the array as the "pivot." Different strategies can be used to pick the pivot, such as selecting the first element, the last element, a random element, or the middle element. The choice of pivot affects the efficiency of the algorithm.

- **Partition the array**: Rearrange the array so that all elements less than the pivot are on its left, and all elements greater than the pivot are on its right. After this partition, the pivot is in its correct sorted position.

- **Recursively apply**: Recursively apply the same process to the sub-arrays (elements to the left and right of the pivot) until the entire array is sorted.

## Pseudo code of Quick Sort with Detailed Steps:
```text
QuickSort(arr, low, high) {
    # Check if the range if the range > 1
    if (low < high) {
        int pIndex = partition(arr, low, high);
        # left sub array
        QuickSort(arr, low, pIndex - 1);
        # right sub array
        QuickSort(arr, pIndex + 1, high);
    }
}
int partition(arr, low, high) {
    int pivot = arr[low];
    int i = low;
    int j = high;

    while (i < j) {
        while (arr[i] <= pivot && i <= high - 1) {
            i++;
        }

        while (arr[j] > pivot && j >= low + 1) {
            j--;
        }
        if (i < j) swap(arr[i], arr[j]);
    }
    swap(arr[low], arr[j]);
    return j;
}


```
### Explanation:

1. **quickSort Function**:
The quickSort function is called recursively on two sub-arrays: one before the pivot (arr[low] to arr[pivotIndex - 1]) and one after the pivot (arr[pivotIndex + 1] to arr[high]).
The recursion continues until the sub-arrays are reduced to a size of 1 or 0, at which point the array is sorted.

2. **partition Function**:
The partition function rearranges the array around a chosen pivot.
It ensures that elements smaller than the pivot come before it, and elements larger than the pivot come after it.
After partitioning, the pivot is in its correct sorted position, and the function returns the index of the pivot.

## Time and Space Complexity (Short Version)

#### **Time Complexity**:
- **Best/Average Case (O(n log n))**: The array is divided well, so it takes O(n log n) time.
- **Worst Case (O(n²))**: If the pivot is always the smallest or largest, it takes O(n²) time.

#### **Space Complexity**:
- **Best/Average Case (O(log n))**: Only the recursion stack uses space, so it's O(log n).
- **Worst Case (O(n))**: In the worst case, the recursion stack can go as deep as n, so it's O(n).

## Practice Problems
- [Sort an array - LeetCode](https://leetcode.com/problems/sort-an-array/)  



