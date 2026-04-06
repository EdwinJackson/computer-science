# Maximum Subarray
Difficulty: **Medium** (Often classified as Easy on LeetCode)

Requirements:
- Given an integer array `nums`.
- Find the contiguous subarray (containing at least one number) which has the largest sum.
- Return the sum of that subarray.

Test cases:
```js
maxSubArray([-2, 1, -3, 4, -1, 2, 1, -5, 4]) // returns 6 (from subarray [4, -1, 2, 1])
maxSubArray([1]) // returns 1
maxSubArray([5, 4, -1, 7, 8]) // returns 23 (from the whole array)
maxSubArray([-1]) // returns -1
maxSubArray([-2, -1]) // returns -1 (from subarray [-1])
```

JavaScript Solution

```js
/**
 * @param {number[]} nums
 * @return {number}
 */
var maxSubArray = function(nums) {
    if (!nums || nums.length === 0) {
        // Or throw an error, depending on how invalid input should be handled
        return 0;
    }

    let currentMax = nums[0]; // Max sum ending at the current position
    let globalMax = nums[0];  // Max sum found overall so far

    for (let i = 1; i < nums.length; i++) {
        // Decide whether to extend the existing subarray or start a new one
        currentMax = Math.max(nums[i], currentMax + nums[i]);

        // Update the overall maximum sum if the current subarray's sum is greater
        globalMax = Math.max(globalMax, currentMax);
    }

    return globalMax;
};
```

## Related To
- [[data structures/Arrays]]
