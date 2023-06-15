Ordering and searching are two fundamental computer science concepts essential for storing, organizing, and accessing data efficiently. 

## Ordering
Ordering is the process of arranging data in a certain way, such as ascending, descending, alphabetical, or numerical order. Ordering makes it easier to find, compare, and manipulate data. Structuring our data improves predictability and helps us retrieve information quickly and accurately. For example, if you have a list of names, ordering them alphabetically can help you locate a specific name faster than if they were in random order.

### Sorting algorithms
These are algorithms that order a collection of data in a certain way. Sorting algorithms have different time and space complexities depending on how they work and how efficient they are.

- [[Bubble Sort]] - a simple but slow algorithm that compares adjacent elements and swaps them if they are out of order.
	- time complexity $O(n^2)$ 
	- space complexity $O(1)$.
- [[Insertion Sort]] - a simple sorting algorithm that works by building a sorted list one element at a time. 
	- time complexity $O(n^2)$ 
	- space complexity $O(1)$
- [[Merge Sort]] - Merge sort is a sorting algorithm that works by dividing an array into smaller subarrays, sorting each subarray, and then merging the sorted subarrays back together to form the final sorted array. 
	- time complexity of $O(n log(n))$ 
		- space complexity of $O(n)$  
- [[Quick Sort]] - a sorting algorithm that uses the divide-and-conquer strategy around a pivot. 
	- time complexity $O(n^2)$ 
	- space complexity $O(1)$
- [[Heap Sort]] - organizes elements in an array into a binary heap, a special kind of complete binary tree where each node is greater than or equal to its children. 
	- time complexity $O(n*log(n))$ 
	- space complexity $O(log(n))$

### Data Structures
- [[Hash Table]]: These are data structures that store data in key-value pairs using a hash function to map each key to an index in an array. 
- [[Binary Search Tree]]: Binary search trees maintain an order among the nodes such that the left child of a node is smaller than the node and the right child is larger than the node

## Searching
Searching is the process of finding a specific piece of data within a collection of data. This process is widely used in various applications, including search engines, databases, and file systems, to locate and retrieve relevant information. Searching can be done in different ways depending on how the data is ordered and stored. For example, if you have an ordered array of numbers, you can use a binary search algorithm to find a target number by repeatedly dividing the array into two halves and comparing the target with the middle element. Another example is searching for a word in a dictionary by using the first letter as the search criterion.

### Searching Algorithms
- [[Linear Search]] - This is a simple searching algorithm that scans through a collection of data from left to right until it finds the target or reaches the end. It is inefficient for large collections.
- [[Binary Search]]- This is a fast and efficient searching algorithm that works on ordered collections of data, it does not work on unordered data. Binary search repeatedly divides the collection into two halves and compares the target with the middle element until it finds the target or determines that it does not exist.