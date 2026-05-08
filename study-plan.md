# Computer Science Concepts

Sometimes it's really good to just cover the basics. You can find some examples of core concepts and brief explanations on them ideally with some sort of diagram, image, or video.

# Study Plan

**Core Principles:**

1.  **Consistency:** Aim to study and practice regularly (e.g., daily or several times a week).
2.  **Understanding over Memorization:** Focus on *why* a particular data structure or algorithm works and is chosen for a problem.
3.  **Start Simple, Build Complexity:** Begin with easier problems within a topic to grasp the fundamentals before tackling medium/hard ones.
4.  **Complexity Analysis:** Always analyze the time and space complexity (Big O notation) of your solutions. Interviewers *will* ask.
5.  **Practice Communication:** Try explaining your thought process out loud as you solve problems.

**Suggested Timeline:** 8-12 Weeks (Flexible - adjust based on your pace and available time)

---

**Phase 1: Foundations (Weeks 1-2)**

* **Week 1: Big O Notation & Arrays/Strings**
    * **Concepts:** Time Complexity, Space Complexity, Big O Notation (O(1), O(log n), O(n), O(n log n), O(n^2), O(2^n)). Basic array/string operations (access, insertion, deletion, iteration).
    * **LeetCode Focus:**
        * **Arrays:** Two Sum (Easy), Best Time to Buy and Sell Stock (Easy), Contains Duplicate (Easy), Product of Array Except Self (Medium), Maximum Subarray (Medium).
        * **Strings:** Valid Palindrome (Easy), Valid Anagram (Easy), Longest Substring Without Repeating Characters (Medium), Group Anagrams (Medium).
    * **Tips:** Understand how nested loops affect complexity. Learn common string manipulation methods in your chosen language.

* **Week 2: Hash Tables (Hash Maps / Dictionaries)**
    * **Concepts:** Hash functions, collision handling, key-value storage, average O(1) lookups/insertions/deletions.
    * **LeetCode Focus:**
        * Revisit: Two Sum, Contains Duplicate, Valid Anagram, Group Anagrams (often solved efficiently with hash tables).
        * New: Ransom Note (Easy), First Unique Character in a String (Easy), Subarray Sum Equals K (Medium), Top K Frequent Elements (Medium - may also use Heaps later).
    * **Tips:** Hash tables are extremely common for counting frequencies, checking existence, and mapping values. Recognize when a problem can be simplified using quick lookups.

---

**Phase 2: Core Data Structures (Weeks 3-5)**

* **Week 3: Linked Lists**
    * **Concepts:** Singly linked lists, doubly linked lists, nodes, pointers/references, traversal, insertion, deletion. Sentinel nodes. Fast/slow pointer technique.
    * **LeetCode Focus:**
        * Reverse Linked List (Easy), Merge Two Sorted Lists (Easy), Palindrome Linked List (Easy), Linked List Cycle (Easy - Fast/Slow Pointers), Remove Nth Node From End of List (Medium), Reorder List (Medium).
    * **Tips:** Draw linked lists! Visualizing the pointer manipulation is crucial. Practice both iterative and recursive solutions where applicable.

* **Week 4: Stacks & Queues**
    * **Concepts:** Stack (LIFO - Last In First Out), Queue (FIFO - First In First Out). Common operations (push, pop, peek, enqueue, dequeue). Applications (parsing, BFS, etc.).
    * **LeetCode Focus:**
        * **Stacks:** Valid Parentheses (Easy), Min Stack (Easy), Evaluate Reverse Polish Notation (Medium), Daily Temperatures (Medium).
        * **Queues:** Implement Stack using Queues (Easy), Implement Queue using Stacks (Easy), Number of Islands (Medium - uses Queue for BFS, see Graphs week), Design Circular Queue (Medium).
    * **Tips:** Recognize problems where order of processing matters (LIFO/FIFO). Stacks are great for matching pairs or reversing order. Queues are fundamental for level-order traversal (BFS).

* **Week 5: Trees (Binary Trees & Binary Search Trees - BSTs)**
    * **Concepts:** Nodes, root, parent, child, leaf. Tree traversals (Inorder, Preorder, Postorder - recursive and iterative). Level-order traversal (BFS). Binary Search Tree properties, insertion, validation, searching. Height, depth, balancing (conceptual).
    * **LeetCode Focus:**
        * **General Trees:** Maximum Depth of Binary Tree (Easy), Same Tree (Easy), Invert Binary Tree (Easy), Binary Tree Level Order Traversal (Medium), Construct Binary Tree from Preorder and Inorder Traversal (Medium).
        * **BSTs:** Validate Binary Search Tree (Medium), Lowest Common Ancestor of a BST (Easy), Kth Smallest Element in a BST (Medium).
    * **Tips:** Recursion is very natural for tree problems. Master the different traversal methods. Understand the BST property deeply.

---

**Phase 3: Algorithms & Advanced Topics (Weeks 6-9)**

* **Week 6: Searching & Sorting + Heaps (Priority Queues)**
    * **Concepts:** Binary Search (on sorted arrays/search spaces). Basic sorting algorithms (conceptual understanding of Bubble, Insertion, Selection, Merge Sort, Quick Sort - know their complexities). Heaps (Min-Heap, Max-Heap), heapify, insert, extract-min/max. Priority Queue applications.
    * **LeetCode Focus:**
        * **Binary Search:** Binary Search (Easy), Find Minimum in Rotated Sorted Array (Medium), Search in Rotated Sorted Array (Medium), Time Based Key-Value Store (Medium).
        * **Heaps:** Kth Largest Element in an Array (Medium), Top K Frequent Elements (Medium), Find Median from Data Stream (Hard), Merge K Sorted Lists (Hard).
        * **Sorting:** Problems often require sorting as a first step (e.g., Merge Intervals (Medium), Meeting Rooms II (Medium) - often solved with sorting + heaps/pointers).
    * **Tips:** Binary search requires a sorted input or a monotonic search space. Heaps are perfect for finding min/max elements efficiently or maintaining order among dynamic elements.

* **Week 7: Graphs**
    * **Concepts:** Nodes (vertices), edges. Representations (Adjacency List, Adjacency Matrix). Traversal algorithms: Breadth-First Search (BFS), Depth-First Search (DFS - recursive and iterative). Connected components, cycles.
    * **LeetCode Focus:**
        * Number of Islands (Medium - BFS or DFS), Clone Graph (Medium - BFS or DFS), Course Schedule (Medium - DFS/Topological Sort), Pacific Atlantic Water Flow (Medium - BFS or DFS from edges), Word Ladder (Hard - BFS).
    * **Tips:** Adjacency lists are usually preferred. Choose BFS for shortest paths in unweighted graphs and level-order traversal. Choose DFS for exploring paths fully, cycle detection, and topological sort. Practice building the graph representation from the problem description.

* **Week 8: Recursion & Backtracking**
    * **Concepts:** Base cases, recursive steps. Exploring all possible solutions/combinations/permutations. Pruning the search space.
    * **LeetCode Focus:**
        * Subsets (Medium), Combination Sum (Medium), Permutations (Medium), N-Queens (Hard), Word Search (Medium).
    * **Tips:** Backtracking often involves a helper function with parameters tracking the current state. Use a "choose, explore, unchoose" pattern. Draw the recursion tree to understand the flow.

* **Week 9: Dynamic Programming (DP)**
    * **Concepts:** Overlapping subproblems, optimal substructure. Memoization (top-down) vs. Tabulation (bottom-up). Identifying DP state and recurrence relation.
    * **LeetCode Focus:**
        * Climbing Stairs (Easy), Coin Change (Medium), Longest Increasing Subsequence (Medium), House Robber (Medium), Word Break (Medium), Edit Distance (Hard).
    * **Tips:** DP can be challenging. Start with problems that have clear overlapping subproblems. Try solving recursively first, then add memoization. Finally, try converting to a bottom-up tabulation approach. Practice recognizing DP patterns.

---

**Phase 4: Common Patterns & Review (Weeks 10-12+)**

* **Week 10: Common Algorithmic Patterns**
    * **Concepts:** Two Pointers, Sliding Window, Greedy Algorithms.
    * **LeetCode Focus:**
        * **Two Pointers:** Valid Palindrome (Easy), Container With Most Water (Medium), 3Sum (Medium), Trapping Rain Water (Hard).
        * **Sliding Window:** Best Time to Buy and Sell Stock (Easy), Longest Substring Without Repeating Characters (Medium), Minimum Window Substring (Hard).
        * **Greedy:** Maximum Subarray (Medium - Kadane's algorithm), Jump Game (Medium), Merge Intervals (Medium).
    * **Tips:** Recognize when comparing/manipulating elements from both ends (Two Pointers) or analyzing contiguous subarrays/substrings (Sliding Window) is beneficial. Greedy works when making the locally optimal choice leads to a global optimum.

* **Week 11: Review & Practice Mediums**
    * **Focus:** Revisit topics you found difficult. Solve a variety of Medium-level problems mixing different data structures and algorithms. Check company-specific tagged LeetCode lists if you are targeting particular companies.
    * **Activity:** Try mock interviews ( platforms like Pramp or interviewing.io, or practice with peers). Focus on clearly explaining your approach *before* coding and discussing trade-offs.

* **Week 12+: Advanced Topics & Mock Interviews**
    * **Concepts (Optional/If Time Permits):** Tries (Prefix Trees), Bit Manipulation, Advanced Graph Algorithms (Dijkstra's, Floyd-Warshall), Union-Find.
    * **LeetCode Focus:**
        * **Tries:** Implement Trie (Prefix Tree) (Medium), Design Add and Search Words Data Structure (Medium).
        * **Bit Manipulation:** Number of 1 Bits (Easy), Single Number (Easy), Reverse Bits (Easy).
        * **Union-Find:** Number of Connected Components in an Undirected Graph (Medium).
    * **Activity:** Continue solving Medium/Hard problems. Do more timed mock interviews simulating real conditions. Review common behavioral questions as well.

---

**Final Tips:**

* **LeetCode Problem Selection:** Filter problems by frequency or company tags if desired. Start with Easy, but quickly move to Mediums as they are most common in interviews. Tackle Hards once comfortable with Mediums.
* **Don't Look at Solutions Too Quickly:** Spend adequate time (e.g., 20-40 minutes) struggling with a problem before looking at hints or solutions.
* **Understand Solutions:** If you look at a solution, don't just copy it. Understand *why* it works, its complexity, and try to re-implement it yourself later. Read the discussion forums for different approaches.
* **Stay Updated:** Interview trends can shift slightly. Keep an eye on resources like LeetCode Discuss or Blind for recent experiences.

Good luck with your preparation! Remember that consistent effort is the most important factor.
