# Valid Anagram
Difficulty: **Easy**

Requirements:
- Given two strings `s` and `t`.
- Return `true` if `t` is an anagram of `s`, and `false` otherwise.
- An anagram is formed by rearranging the letters of a word, using all original letters exactly once.

Test cases:
```js
isAnagram("anagram", "nagaram") // returns true
isAnagram("rat", "car") // returns false
isAnagram("listen", "silent") // returns true
isAnagram("a", "ab") // returns false
isAnagram("", "") // returns true
isAnagram("aacc", "ccac") // returns false (counts don't match 'a')
```

## JavaScript Solution

```js
/**
 * @param {string} s
 * @param {string} t
 * @return {boolean}
 */
var isAnagram = function(s, t) {
    // 1. Anagrams must have the same length
    if (s.length !== t.length) {
        return false;
    }

    // 2. Create a frequency map for string s
    const charCount = {}; // Or new Map()

    for (const char of s) {
        charCount[char] = (charCount[char] || 0) + 1;
    }

    // 3. Decrement counts based on string t
    for (const char of t) {
        // If char from t is not in s's map, or count is already 0
        if (!charCount[char]) {
            return false;
        }
        charCount[char]--;
    }

    // 4. If we reached here, all characters in t were accounted for
    // and since lengths are equal, it must be an anagram.
    // (No need to check if all counts are zero, as the length check
    // and the decrement logic ensure this if the loop completes).
    return true;
};

// Alternative using sorting (less efficient time complexity O(n log n))
var isAnagramSort = function(s, t) {
    if (s.length !== t.length) {
        return false;
    }
    return s.split('').sort().join('') === t.split('').sort().join('');
};
```

## Related To
- [[data structures/Hash Table]]
- [[algorithms/Merge Sort]]
