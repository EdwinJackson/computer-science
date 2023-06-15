Selection sort is a sorting algorithm that repeatedly finds the minimum element from the unsorted part of an array and moves it to the sorted part. The algorithm maintains two subarrays in a given array: one that is already sorted and one that is unsorted. In every iteration, the algorithm selects the smallest element from the unsorted subarray and swaps it with the leftmost element of that subarray, moving the boundary of the sorted subarray by one element. The algorithm stops when the unsorted subarray becomes empty.

The time complexity of selection sort is O(n^2), where n is the number of elements in the array. This is because the algorithm performs n-1 comparisons for the first element, n-2 comparisons for the second element, and so on, until one comparison for the last element. The total number of comparisons is (n-1) + (n-2) + ... + 1 = n(n-1)/2, which is O(n^2) in asymptotic notation. The space complexity of selection sort is `O(1)` since it only uses a constant amount of extra space for swapping elements.

## Specs
|      | Time   | Space |
| ---- | ------ | ----- |
| Best | `O(n^2)` | `O(1)`  | 

The total number of comparisons is `(n-1) + (n-2) + ... + 1 = n(n-1)/2`, which is `O(n^2)` in asymptotic notation.

The time complexity of Selection Sort is `O(n^2)`, where n is the number of elements in the array. This is because the algorithm performs n-1 comparisons for the first element, `n-2` comparisons for the second element, and so on, until one comparison for the last element. 

## Visual
![[selection-sort.excalidraw.svg]]

## Implementation

```ts
function selectionSort(array: number[]): number[] {
  const len = array.length;

  for (let i = 0; i < len - 1; i++) {
    let minIndex = i;

    for (let j = i + 1; j < len; j++) {
      if (array[j] < array[minIndex]) {
        minIndex = j;
      }
    }

    if (minIndex !== i) {
      [array[i], array[minIndex]] = [array[minIndex], array[i]]; // Swap elements using destructuring assignment
    }
  }

  return array;
}

const unsortedArray = [4, 2, 7, 1, 5];
const sortedArray = selectionSort(unsortedArray);
console.log(sortedArray); // Output: [1, 2, 4, 5, 7]
```

-   The `selectionSort` function takes an array of numbers called `array` as input and returns the sorted array.
-   The `len` variable stores the length of the array.
-   The outer loop iterates from `i = 0` to `len - 1` to select the smallest element in each pass.
-   The `minIndex` variable keeps track of the index of the current minimum element, initially set to `i`.
-   The inner loop iterates from `j = i + 1` to `len` and compares each element with the current minimum element.
-   If a smaller element is found, the `minIndex` is updated to the index of that element.
-   After completing the inner loop, if the `minIndex` is not the same as `i`, the current element and the minimum element are swapped using destructuring assignment `[a, b] = [b, a]`.
-   Finally, the sorted array is returned.

## Related To:
- [[Order & Search]]
- [[Binary Search]]
- [[Heap Sort]]
- [[Merge Sort]]
- [[Quick Sort]]
- [[Bubble Sort]]