# Two Sum

Difficulty: **Easy**

Requirements:
- Given an array of integers `nums` and an integer `target`.
- Return indices of the two numbers in the array such that they add up to `target`.
- You may assume that each input would have exactly one solution.
- You may not use the same element twice.
- You can return the answer in any order.

Test cases:
```js
twoSum([2, 7, 11, 15], 9) // returns [0, 1] (because nums[0] + nums[1] == 9)
twoSum([3, 2, 4], 6) // returns [1, 2] (because nums[1] + nums[2] == 6)
twoSum([3, 3], 6) // returns [0, 1] (because nums[0] + nums[1] == 6)
```

```js
/**
 * @param {number[]} nums
 * @param {number} target
 * @return {number[]}
 */
var twoSum = function(nums, target) {
    const map = new Map(); // Use a Map to store number -> index

    for (let i = 0; i < nums.length; i++) {
        const complement = target - nums[i];

        // Check if the complement exists in the map
        if (map.has(complement)) {
            // Found the pair
            return [map.get(complement), i];
        }

        // Add the current number and its index to the map
        map.set(nums[i], i);
    }

    // No solution found (though the problem statement guarantees one)
    // This line is theoretically unreachable based on problem constraints
    return [];
};
```
