# Group Anagrams
Difficulty: **Medium**

Requirements:
- Given an array of strings `strs`.
- Group the anagrams together.
- You can return the answer (the groups of anagrams) in any order.

Test cases:
```js
groupAnagrams(["eat","tea","tan","ate","nat","bat"])
// returns [["bat"],["nat","tan"],["ate","eat","tea"]] (order of groups and strings within groups doesn't matter)

groupAnagrams([""])
// returns [[""]]

groupAnagrams(["a"])
// returns [["a"]]

groupAnagrams(["abc", "bca", "bac", "xyz", "zyx"])
// returns [["abc","bca","bac"], ["xyz","zyx"]]
```

## Solution

```js
/**
 * @param {string[]} strs
 * @return {string[][]}
 */
function groupAnagrams(strs) {
    // Map to store anagram groups
    // Key: sorted version of the string (anagram signature)
    // Value: array of original strings belonging to that group
    const anagramMap = new Map();

    for (const str of strs) {
        // Create the signature by sorting the string
        const sortedStr = str.split('').sort().join('');

        // If the signature isn't in the map, initialize an empty array
        if (!anagramMap.has(sortedStr)) {
            anagramMap.set(sortedStr, []);
        }

        // Add the original string to the list for this signature
        anagramMap.get(sortedStr).push(str);
    }

    // The values of the map are the grouped anagrams
    return Array.from(anagramMap.values());
};
```

Alternative using character count as key (more complex key generation)

```js
function groupAnagramsCharCount(strs) {
    const anagramMap = new Map();

    for (const str of strs) {
        // Create a frequency count array (size 26 for 'a' through 'z')
        const count = new Array(26).fill(0);
        for (let i = 0; i < str.length; i++) {
            // Calculate index based on character code ('a' is 97)
            const charIndex = str.charCodeAt(i) - 97;
            count[charIndex]++;
        }

        // Create a string key from the count array (e.g., "1#0#2#...")
        const key = count.join('#'); // Use a separator

        if (!anagramMap.has(key)) {
            anagramMap.set(key, []);
        }
        anagramMap.get(key).push(str);
    }

    return Array.from(anagramMap.values());
};
```

## Related To
- [[data structures/Hash Table]]
- [[algorithms/Merge Sort]]
