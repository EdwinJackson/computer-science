# Contains Duplicate
Difficulty: **Easy**

Requirements:
- Given an integer array `nums`.
- Return `true` if any value appears at least twice in the array.
- Return `false` if every element is distinct.

Test cases:
```js
containsDuplicate([1, 2, 3, 1]) // returns true
containsDuplicate([1, 2, 3, 4]) // returns false
containsDuplicate([1, 1, 1, 3, 3, 4, 3, 2, 4, 2]) // returns true
containsDuplicate([]) // returns false
containsDuplicate([5]) // returns false
```

JavaScript Solution

```js
/**
 * @param {number[]} nums
 * @return {boolean}
 */
var containsDuplicate = function(nums) {
    const seen = new Set(); // Use a Set for efficient O(1) average time lookups

    for (const num of nums) {
        if (seen.has(num)) {
            // Duplicate found
            return true;
        }
        seen.add(num); // Add the number to the set
    }

    // No duplicates found after checking all numbers
    return false;
};
```
