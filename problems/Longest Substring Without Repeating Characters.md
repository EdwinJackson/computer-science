# Longest Substring Without Repeating Characters
Difficulty: **Medium**

Requirements:
- Given a string `s`.
- Find the length of the longest substring within `s` that does not contain repeating characters.
- A substring is a contiguous sequence of characters within a string.

Test cases:
```js
lengthOfLongestSubstring("abcabcbb") // returns 3 (substring "abc")
lengthOfLongestSubstring("bbbbb") // returns 1 (substring "b")
lengthOfLongestSubstring("pwwkew") // returns 3 (substring "wke")
lengthOfLongestSubstring("") // returns 0
lengthOfLongestSubstring(" ") // returns 1
lengthOfLongestSubstring("au") // returns 2
lengthOfLongestSubstring("dvdf") // returns 3 (substring "vdf")
```

<details>
<summary>JavaScript Solution</summary>

```js
/**
 * @param {string} s
 * @return {number}
 */
var lengthOfLongestSubstring = function(s) {
    let maxLength = 0;
    let left = 0; // Left pointer of the sliding window
    // Map stores the character and its *last seen index* + 1
    const charMap = new Map();

    for (let right = 0; right < s.length; right++) {
        const currentChar = s[right];

        // If the character is already in the map AND its last occurrence
        // is within the current window (i.e., its index >= left pointer)
        // then we need to move the left pointer past the previous occurrence.
        if (charMap.has(currentChar) && charMap.get(currentChar) >= left) {
            left = charMap.get(currentChar) + 1;
        }

        // Update the last seen index for the current character
        charMap.set(currentChar, right);

        // Calculate the length of the current window
        const currentLength = right - left + 1;

        // Update the maximum length found so far
        maxLength = Math.max(maxLength, currentLength);
    }

    return maxLength;
};

```
Alternative using a Set (slightly different window update logic)

```js
const lengthOfLongestSubstringSet = function(s) {
    let left = 0;
    let right = 0;
    let maxLength = 0;
    const charSet = new Set();

    while (right < s.length) {
        const currentChar = s[right];
        if (!charSet.has(currentChar)) {
            // Character not in window, expand window to the right
            charSet.add(currentChar);
            maxLength = Math.max(maxLength, right - left + 1);
            right++;
        } else {
            // Character IS in window, shrink window from the left
            charSet.delete(s[left]);
            left++;
        }
    }
    return maxLength;
};
```

</details>
