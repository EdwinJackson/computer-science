Heap sort is a sorting algorithm that organizes elements in an array into a binary heap, a special kind of complete binary tree where each node is greater than or equal to its children. The algorithm works by repeatedly moving the largest element from the heap to the end of the array, and then reducing the size of the heap by one. This process is called `heapify`, and it ensures that the remaining elements in the heap are always in the correct order.

The heap sort algorithm can be described as follows:

1. Build a max-heap from the input array. This can be done by starting from the last non-leaf node (at `index n/2 - 1`) and calling `heapify` on it and all its ancestors in reverse order.
2. Swap the root of the heap (the largest element) with the last element of the array.
3. Reduce the size of the heap by one and call `heapify` on the root to restore the heap property.
4. Repeat steps 2 and 3 until the heap size is one.

The `heapify` function takes an array, a node index, and a heap size as parameters, and it does the following:

1. Find the largest among the node, its left child (at index `2*i + 1`), and its right child (at index `2*i + 2`).
2. If the largest is not the node, swap it with the node and recursively call `heapify` on the swapped child.

## Specs
|      | Time        | Space     |
| ---- | ----------- | --------- |
| Best | $O(n log(n))$ | $O(log(n))$ |

## Visual

## Implementation
```ts
function heapSort(array: number[]): number[] {
  const len = array.length;

  // Build max heap
  for (let i = Math.floor(len / 2) - 1; i >= 0; i--) {
    heapify(array, len, i);
  }

  // Heap sort
  for (let i = len - 1; i > 0; i--) {
    // Swap root (max) with the last element
    [array[0], array[i]] = [array[i], array[0]]; 
    // Heapify the reduced heap
    heapify(array, i, 0);
  }

  return array;
}

function heapify(array: number[], heapSize: number, rootIndex: number) {
  let largest = rootIndex;
  const leftIndex = 2 * rootIndex + 1;
  const rightIndex = 2 * rootIndex + 2;

  if (leftIndex < heapSize && array[leftIndex] > array[largest]) {
    largest = leftIndex;
  }

  if (rightIndex < heapSize && array[rightIndex] > array[largest]) {
    largest = rightIndex;
  }

  if (largest !== rootIndex) {
    // Swap elements using destructuring assignment
    [array[rootIndex], array[largest]] = [array[largest], array[rootIndex]];
    // Recursively heapify the affected sub-tree
    heapify(array, heapSize, largest);
  }
}

const unsortedArray = [4, 2, 7, 1, 5];
const sortedArray = heapSort(unsortedArray);
console.log(sortedArray); // Output: [1, 2, 4, 5, 7]
```

-   The `heapSort` function takes an array of numbers called `array` as input and returns the sorted array.
-   The `len` variable stores the length of the array.
-   The `heapify` function is used to heapify a subtree rooted at `rootIndex` within the `array`.
-   The `heapify` function compares the root element with its left and right child (if they exist) and swaps the root with the largest element if necessary.
-   The `heapSort` function first builds a max heap by calling `heapify` for all non-leaf nodes in the array.
-   Then, it performs the heap sort by repeatedly swapping the root (maximum element) with the last element in the array, reducing the heap size, and heapifying the reduced heap.
-   Finally, the sorted array is returned.

## Relates To
- [[Order & Search]]
- [[Selection Sort]]
- [[Insertion Sort]]
- [[Merge Sort]]
- [[Quick Sort]]
- [[Bubble Sort]]