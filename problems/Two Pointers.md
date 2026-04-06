# Reverse String
Difficulty: **Easy**

**The Scenario:** You are developing a **Low-Level Protocol Driver** for a legacy telecommunications system. Data packets are arriving in "Big-Endian" byte order, but the local hardware architecture requires "Little-Endian" processing for specific fixed-length header strings.

- **The Goal:** Invert the sequence of characters in the header string in-place to minimize memory overhead on the embedded chip.

## Requirements
- Write a function that reverses a string. The input string is given as an array of characters `s`.
- You must do this by modifying the input array in-place with O(1) extra memory.

## Test Cases
```js
reverseString(["h","e","l","l","o"]) // ["o","l","l","e","h"]
reverseString(["H","a","n","n","a","h"]) // ["h","a","n","n","a","H"]
```

## Solution

```ts
/**
 Do not return anything, modify s in-place instead.
 */
function reverseString(s: string[]): void {
    let left = 0;
    let right = s.length - 1;

    while (left < right) {
        // Swap characters
        [s[left], s[right]] = [s[right], s[left]];
        left++;
        right--;
    }
}
```

## Related To
- [[data structures/Arrays]]
