# Search in Rotated Sorted Array
Difficulty: **Medium**

**The Scenario:** You are managing a **Log Rotation System** for a global server cluster. The logs were originally sorted by timestamp, but due to a server restart and "wrapping" logic, the oldest logs moved to the middle, and the newest logs started again at the beginning (e.g., `[5, 6, 7, 0, 1, 2, 4]`).

- **The Goal:** Find the exact index of a specific timestamp in $O(\log n)$ time so the system can quickly retrieve an error log without scanning the entire disk.

## Requirements
- There is an integer array `nums` sorted in ascending order (with distinct values).
- Prior to being passed to your function, `nums` is possibly rotated at an unknown pivot index `k` (`1 <= k < nums.length`) such that the resulting array is `[nums[k], nums[k+1], ..., nums[n-1], nums[0], nums[1], ..., nums[k-1]]` (0-indexed).
- Given the array `nums` after the possible rotation and an integer `target`, return the index of `target` if it is in `nums`, or `-1` if it is not in `nums`.
- You must write an algorithm with $O(\log n)$ runtime complexity.

## Test Cases
```js
search([4,5,6,7,0,1,2], 0) // returns 4
search([4,5,6,7,0,1,2], 3) // returns -1
search([1], 0) // returns -1
```

## Solution

```ts
function search(nums: number[], target: number): number {
    let left = 0;
    let right = nums.length - 1;

    while (left <= right) {
        const mid = Math.floor((left + right) / 2);

        if (nums[mid] === target) return mid;

        // Check if the left half is sorted
        if (nums[left] <= nums[mid]) {
            if (nums[left] <= target && target < nums[mid]) {
                right = mid - 1; // Target is in the left half
            } else {
                left = mid + 1; // Target is in the right half
            }
        }
        // Otherwise, the right half must be sorted
        else {
            if (nums[mid] < target && target <= nums[right]) {
                left = mid + 1; // Target is in the right half
            } else {
                right = mid - 1; // Target is in the left half
            }
        }
    }

    return -1;
}
```

## Related To
- [[algorithms/Binary Search]]
- [[data structures/Arrays]]
