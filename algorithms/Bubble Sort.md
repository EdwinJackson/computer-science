Bubble sort is a simple sorting algorithm that compares adjacent elements and swaps them if they are out of order. The algorithm repeats this process until the array is sorted. 

## Specs
|       | Time   | Space |
| ----- | ------ | ----- |
| Best  | $O(n)$   | $O(1)$  |
| Worst | $O(n^2)$ | -     | 

## Visual
![[bubble-sort.excalidraw.svg]]

## Implementation

```ts
function bubbleSort(array: number[]): number[] {
  const len = array.length;

  for (let i = 0; i < len - 1; i++) {
    let swapped = false;

    for (let j = 0; j < len - 1 - i; j++) {
      if (array[j] > array[j + 1]) {
        [array[j], array[j + 1]] = [array[j + 1], array[j]]; // Swap elements using destructuring assignment
        swapped = true;
      }
    }

    if (!swapped) {
      break; // Optimization: If no swaps were made in a pass, the array is already sorted
    }
  }

  return array;
}

const unsortedArray = [4, 2, 7, 1, 5];
const sortedArray = bubbleSort(unsortedArray);
console.log(sortedArray); // Output: [1, 2, 4, 5, 7]
```

-   The `bubbleSort` function takes an array of numbers called `array` as input and returns the sorted array.
-   The `len` variable stores the length of the array.
-   The outer loop iterates from `i = 0` to `len - 1` to perform `len - 1` passes.
-   The inner loop iterates from `j = 0` to `len - 1 - i` and compares adjacent elements.
-   If the current element is greater than the next element, they are swapped using destructuring assignment `[a, b] = [b, a]`.
-   The `swapped` flag keeps track of whether any swaps were made in a pass. If no swaps were made, it means the array is already sorted, and the loop breaks to optimize the algorithm.
-   Finally, the sorted array is returned.

## Related To:
- [[Order & Search]]
- [[Selection Sort]]
- [[Insertion Sort]]
- [[Heap Sort]]
- [[Merge Sort]]
- [[Quick Sort]]