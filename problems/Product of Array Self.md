# Product of Array Except Self
Difficulty: **Medium**

Requirements:
- Given an integer array `nums`.
- Return an array `answer` such that `answer[i]` is equal to the product of all the elements of `nums` except `nums[i]`.
- The product of any prefix or suffix of `nums` is guaranteed to fit in a 32-bit integer.
- You must write an algorithm that runs in O(n) time.
- You must not use the division operator.
- Bonus: Solve in O(1) extra space complexity (the output array `answer` does not count as extra space).

Test cases:
```js
productExceptSelf([1, 2, 3, 4]) // returns [24, 12, 8, 6]
productExceptSelf([-1, 1, 0, -3, 3]) // returns [0, 0, 9, 0, 0]
productExceptSelf([0, 0]) // returns [0, 0]
productExceptSelf([1, 0]) // returns [0, 1]
```

JavaScript Solution

```js
/**
 * @param {number[]} nums
 * @return {number[]}
 */
var productExceptSelf = function(nums) {
    const n = nums.length;
    const answer = new Array(n).fill(1);

    // Calculate prefix products and store in answer array
    let prefix = 1;
    for (let i = 0; i < n; i++) {
        answer[i] = prefix;
        prefix *= nums[i];
    }

    // Calculate suffix products and multiply with existing prefix products in answer array
    let suffix = 1;
    for (let i = n - 1; i >= 0; i--) {
        answer[i] *= suffix;
        suffix *= nums[i];
    }

    return answer;
};
```
