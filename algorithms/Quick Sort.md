Quicksort is a sorting algorithm that uses the divide-and-conquer strategy. It chooses an element from the array, called the `pivot`, and partitions the array into two subarrays: one with elements smaller than or equal to the `pivot`, and one with elements larger than the `pivot`. Then it recursively sorts the subarrays until the whole array is sorted. Quicksort is an efficient and general-purpose algorithm that can sort any type of data. It is faster than merge sort and heapsort on average, but it can have a worst-case running time of $O(n^2)$ if the pivot is chosen poorly.

## Specs
|       | Time        | Space |
| ----- | ----------- | ----- |
| Best  | $O(n log(n))$ | $O(1)$  |
| Worst | $O(n^2)$    |       |

## Visual
![[quick-sort.excalidraw.svg]]

## Implementation

```ts
function quickSort(array: number[]): number[] {
  if (array.length <= 1) {
    return array;
  }

  // we arbitrarily decide to take the last index
  // you could in theory use any index as the pivot
  // first and last are recommended since they're predictable
  const pivot = array[array.length - 1];
  const left: number[] = [];
  const right: number[] = [];

  for (let i = 0; i < array.length - 1; i++) {
    if (array[i] < pivot) {
      left.push(array[i]);
    } else {
      right.push(array[i]);
    }
  }

  return [...quickSort(left), pivot, ...quickSort(right)];
}

const unsortedArray = [4, 2, 7, 1, 5];
const sortedArray = quickSort(unsortedArray);
console.log(sortedArray); // Output: [1, 2, 4, 5, 7]
```

-   The `quickSort` function takes an array of numbers called `array` as input and returns the sorted array.
-   If the length of the array is less than or equal to 1, it is already sorted, so it is returned as is.
-   The last element of the array is chosen as the pivot element.
-   Two empty arrays, `left` and `right`, are created to hold the elements smaller and greater than the pivot, respectively.
-   The elements of the array are iterated, and each element is pushed into either the `left` or `right` array based on whether it is smaller or greater than the pivot.
-   Finally, the `left` array, pivot, and `right` array are recursively sorted using `quickSort`, and the three arrays are concatenated together to form the sorted array.

## Relates To
- [[Order & Search]]
- [[Heap Sort]]
- [[Selection Sort]]
- [[Insertion Sort]]
- [[Quick Sort]]
- [[Bubble Sort]]