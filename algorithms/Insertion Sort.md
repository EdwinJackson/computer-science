Insertion sort is a simple sorting algorithm that works by building a sorted list one element at a time. It starts with the first element of the input list and compares it with the rest of the elements. If it finds a smaller element, it swaps them. Then it moves to the second element and repeats the process until the end of the list. The result is a sorted list in ascending order.

The main idea of insertion sort is to insert each element into its correct position in the sorted list. To do this, it maintains a pointer to the current element and shifts all the larger elements to the right until it finds the right place to insert the current element. This way, the sorted list grows from left to right and the unsorted list shrinks from right to left.

The time complexity of insertion sort is $O(n^2)$ in the worst case when the input list is in reverse order. In the best case, when the input list is already sorted, it is $O(n)$. The space complexity of insertion sort is $O(1),$ as it only requires a constant amount of extra memory. Insertion sort is stable, meaning that it preserves the relative order of equal elements. It is also adaptive, meaning that it performs better on partially sorted lists.

## Specs
|       | Time     | Space  |
| ----- | -------- | ------ |
| Best  | $O(n)$   | $O(1)$ |
| Worst | $O(n^2)$ |        |

## Visual

## Implementation

```ts
function insertionSort(array: number[]): number[] {
  const len = array.length;

  for (let i = 1; i < len; i++) {
    const current = array[i];
    let prev = i - 1;

    while (prev >= 0 && array[j] > current) {
      array[i] = array[j];
      prev--;
    }

    array[i] = current;
  }

  return array;
}

const unsortedArray = [4, 2, 7, 1, 5];
const sortedArray = insertionSort(unsortedArray);
console.log(sortedArray); // Output: [1, 2, 4, 5, 7]

```

## Related To
- [[Order & Search]]
- [[Selection Sort]]
- [[Heap Sort]]
- [[Merge Sort]]
- [[Quick Sort]]
- [[Bubble Sort]]