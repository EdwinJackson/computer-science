Merge sort is a sorting algorithm that works by dividing an array into smaller subarrays, sorting each subarray, and then merging the sorted subarrays back together to form the final sorted array. The algorithm can be described as follows:

- If the array has zero or one element, it is already sorted and no further steps are needed.
- Otherwise, find the middle index of the array and split it into two subarrays: left and right.
- Recursively apply merge sort to both subarrays.
- Merge the two sorted subarrays into one sorted array by comparing their elements and putting them in order.

The merge operation can be implemented using a temporary array to store the sorted elements, or by using pointers to track the positions of the elements in the original array. 

## Specs
|      | Time        | Space |
| ---- | ----------- | ----- |
| Best | $O(n log(n))$ | $O(n)$  | 

## Visual

## Implementation

```ts
function mergeSort(array: number[]): number[] {
  if (array.length <= 1) {
    return array;
  }

  const mid = Math.floor(array.length / 2);
  const left = mergeSort(array.slice(0, mid));
  const right = mergeSort(array.slice(mid));

  return merge(left, right);
}

function merge(left: number[], right: number[]): number[] {
  const sortedArray: number[] = [];
  let leftIndex = 0;
  let rightIndex = 0;

  while (leftIndex < left.length && rightIndex < right.length) {
    if (left[leftIndex] <= right[rightIndex]) {
      // when left side is lower than right side
      sortedArray.push(left[leftIndex]);
      leftIndex++;
    } else {
      // when right side is lower than left side
      sortedArray.push(right[rightIndex]);
      rightIndex++;
    }
  }

  // Append the remaining elements from left and right subarrays
  while (leftIndex < left.length) {
    sortedArray.push(left[leftIndex]);
    leftIndex++;
  }

  while (rightIndex < right.length) {
    sortedArray.push(right[rightIndex]);
    rightIndex++;
  }

  return sortedArray;
}

const unsortedArray = [4, 2, 7, 1, 5];
const sortedArray = mergeSort(unsortedArray);
console.log(sortedArray); // Output: [1, 2, 4, 5, 7]
```

-   The `mergeSort` function takes an array of numbers called `array` as input and returns the sorted array.
-   If the length of the array is less than or equal to 1, it is already sorted, so it is returned as is.
-   Otherwise, the array is divided into two halves: `left` and `right`, and the `mergeSort` function is called recursively on each half.
-   The `merge` function is responsible for merging the sorted `left` and `right` arrays into a single sorted array.
-   It compares the elements from `left` and `right` and pushes the smaller element into the `sortedArray`.
-   The process continues until all elements from either `left` or `right` are exhausted.
-   Finally, the remaining elements from the non-exhausted array are appended to the `sortedArray`.

## Relates To
- [[Order & Search]]
- [[Heap Sort]]
- [[Selection Sort]]
- [[Insertion Sort]]
- [[Quick Sort]]
- [[Bubble Sort]]