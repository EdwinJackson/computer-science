An array is a data structure that stores a collection of elements of the same type in a contiguous block of memory. Arrays are useful for storing and manipulating data that can be indexed by a numerical position, such as a list of numbers, names, or colours. 

Arrays have a fixed size, meaning that once an array is created, it cannot be resized or expanded. To access an element of an array, we use the array name followed by square brackets containing the index of the element we want. 

```js
const array = ["apple", "banana", "orange"]
console.log(array[0]) // "apple"
console.log(array[array.length]) // undefined
console.log(array[array.length - 1]) // "orange"
```

For example, if we have an array called fruits that contains `["apple", "banana", "orange"]`, we can access the first element by writing `fruits[0]`, which returns `"apple"`. The index of an array starts from zero and goes up to one less than the length of the array. Arrays are one of the most fundamental and widely used data structures in computer science, as they provide a simple and efficient way to store and retrieve data in sequential order.

Seems pretty basic...

## Manipulating Arrays

The efficiency of array operations depends on type, size, and location. Consider common scenarios: insert, delete, modify.

### Insertion
Adding an element to an array is not as easy as one might think. Since arrays are created as a fixed size they need to be expanded in order to accommodate more elements. This gets even more complex when we want to insert an element into the middle of an array, or any position that is not the `array[0]` or `array[array.length -1]` indexes.

**Standard Insertion**
To insert an element at a given position in an array, we need to shift all the elements after that position by one place to the right. This takes $O(n)$ time in the worst case, where n is the number of elements in the array. The space complexity is also $O(n)$, since we may need to allocate a new array if the original one is full.

```java
public class DynamicArray {
    private int[] array;
    private int size;

    public DynamicArray(int initialCapacity) {
        array = new int[initialCapacity];
        size = 0;
    }

    public void insert(int value, int index) {
        if (index < 0 || index > size) {
            throw new IndexOutOfBoundsException("Index out of range: " + index);
        }

        if (size == array.length) {
            resizeArray();
        }

        // Shift elements to the right to accommodate the new value
        for (int i = size; i > index; i--) {
            array[i] = array[i - 1];
        }

        // Insert the value at the specified index
        array[index] = value;
        size++;
    }

    private void resizeArray() {
        int newCapacity = array.length * 2;
        int[] newArray = new int[newCapacity];
        System.arraycopy(array, 0, newArray, 0, size);
        array = newArray;
    }

    public void printArray() {
        for (int i = 0; i < size; i++) {
            System.out.print(array[i] + " ");
        }
        System.out.println();
    }

    public static void main(String[] args) {
        DynamicArray dynamicArray = new DynamicArray(5);
        dynamicArray.insert(10, 0);
        dynamicArray.insert(20, 1);
        dynamicArray.insert(30, 2);
        dynamicArray.insert(40, 1);

        dynamicArray.printArray();  // Output: 10 40 20 30
    }
}
```

In this implementation, the `DynamicArray` class represents an array with dynamic size. The `insert` method takes a value and an index as parameters. It first checks if the index is within the valid range. If the array is full, the `resizeArray` method is called to increase the capacity of the array.

Next, the method shifts the elements to the right from the specified index to create space for the new value. Then it inserts the value at the specified index and increments the size of the array.

The `resizeArray` method creates a new array with double the capacity, copies the elements from the old array to the new array using `System.arraycopy`, and assigns the new array to the `array` reference.

In the `main` method, a `DynamicArray` object is created and values are inserted at different indices. Finally, the `printArray` method is called to display the contents of the array. The output shows the elements of the array after the insertions: `10 40 20 30`.

**Amortized insertion**
Resizing arrays is an expensive operation, amortized insertion helps mitigate that cost. The idea is to double the size of the array when it is full, and then insert the new element. This way, we can insert $n$ elements in $O(n)$ time, which gives an amortized time complexity of $O(1)$ per insertion. The space complexity is also $O(n)$, since we only need to allocate a new array once every $n/2$ insertions.

```java
import java.util.Arrays;

public class DynamicArray {
    private int[] array;
    private int size;

    public DynamicArray(int initialCapacity) {
        array = new int[initialCapacity];
        size = 0;
    }

	// folded
    public void insert(int value, int index) { ... }

    public void bulkInsert(int[] values) {
        if (values == null || values.length == 0) {
            return;
        }

		// double the size of the array
        int newSize = size + values.length;

        if (newSize > array.length) {
            int newCapacity = Math.max(array.length * 2, newSize);
            int[] newArray = Arrays.copyOf(array, newCapacity);
            array = newArray;
        }

        System.arraycopy(array, 0, array, values.length, size);
        System.arraycopy(values, 0, array, 0, values.length);
        size = newSize;
    }

    private void resizeArray() {
        int newCapacity = array.length * 2;
        int[] newArray = new int[newCapacity];
        System.arraycopy(array, 0, newArray, 0, size);
        array = newArray;
    }

	// folded
    public void printArray() { ... }

    public static void main(String[] args) {
        DynamicArray dynamicArray = new DynamicArray(5);
        dynamicArray.insert(10, 0);
        dynamicArray.insert(20, 1);
        dynamicArray.insert(30, 2);
        dynamicArray.insert(40, 1);

        dynamicArray.printArray();  // Output: 10 40 20 30

        int[] valuesToInsert = {50, 60, 70, 80, 90};
        dynamicArray.bulkInsert(valuesToInsert);

        dynamicArray.printArray();  // Output: 50 60 70 80 90 10 40 20 30
    }
}

```

### Deletion
To delete an element at a given position in an array, we need to shift all the elements after that position by one place to the left. This takes $O(n)$ time in the worst case, where n is the number of elements in the array. The space complexity is $O(1)$, since we do not need extra space for deletion.

### Modification
To modify an element at a given position in an array, we simply need to overwrite its value with the new one. This takes $O(1)$ space and time, since we do not need to move any other elements.