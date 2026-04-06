# 3Sum
Difficulty: **Medium**

**The Scenario:** You are building a **FinTech "Expense Bundler"**. A user has a long list of transaction amounts (some positive, some negative). The user wants to find all unique groups of exactly three transactions that, when combined, perfectly cancel each other out (sum to $0$) to help identify potential accounting errors or offsetting entries.

- **The Goal:** Return all unique triplets of transactions that net to zero.

## Requirements
- Given an integer array nums, return all the triplets `[nums[i], nums[j], nums[k]]` such that `i != j`, `i != k`, and `j != k`, and `nums[i] + nums[j] + nums[k] == 0`.
- Notice that the solution set must not contain duplicate triplets.

## Test Cases
```js
threeSum([-1,0,1,2,-1,-4]) // returns [[-1,-1,2],[-1,0,1]]
threeSum([0,1,1]) // returns []
threeSum([0,0,0]) // returns [[0,0,0]]
```

## Solution

```ts
function threeSum(nums: number[]): number[][] {
    const result: number[][] = [];
    if (nums.length < 3) return result;

    // Sort the array to use two pointers technique and handle duplicates easily
    nums.sort((a, b) => a - b);

    for (let i = 0; i < nums.length - 2; i++) {
        // Skip duplicate elements for the first number
        if (i > 0 && nums[i] === nums[i - 1]) continue;

        let left = i + 1;
        let right = nums.length - 1;

        while (left < right) {
            const sum = nums[i] + nums[left] + nums[right];

            if (sum === 0) {
                result.push([nums[i], nums[left], nums[right]]);

                // Skip duplicate elements for the second and third numbers
                while (left < right && nums[left] === nums[left + 1]) left++;
                while (left < right && nums[right] === nums[right - 1]) right--;

                left++;
                right--;
            } else if (sum < 0) {
                left++; // Need a larger sum
            } else {
                right--; // Need a smaller sum
            }
        }
    }

    return result;
}
```

## Related To
- [[data structures/Arrays]]
- [[algorithms/Quick Sort]]
