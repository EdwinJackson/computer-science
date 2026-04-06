# Valid Palindrome
Difficulty: **Easy**

Requirements:
- Given a string `s`.
- Determine if it is a palindrome, considering only alphanumeric characters and ignoring cases.
- An empty string is considered a valid palindrome.

Test cases:
```js
isPalindrome("A man, a plan, a canal: Panama") // returns true
isPalindrome("Kayak") // returns true
isPalindrome("race a car") // returns false
isPalindrome(" ") // returns true (after filtering, it's empty)
isPalindrome("0P") // returns false
isPalindrome("Was it a car or a cat I saw?") // returns true
```

## JavaScript Solution

```js
    /**
 * @param {string} s
 * @return {boolean}
 */
var isPalindrome = function(s) {
    // 1. Filter out non-alphanumeric characters and convert to lowercase
    const cleanedString = s.toLowerCase().replace(/[^a-z0-9]/g, '');

    // An empty string or single character string is a palindrome
    if (cleanedString.length <= 1) {
        return true;
    }

    // 2. Use two pointers
    let left = 0;
    let right = cleanedString.length - 1;

    while (left < right) {
        // 3. Compare characters
        if (cleanedString[left] !== cleanedString[right]) {
            return false; // Characters don't match
        }
        // 4. Move pointers inward
        left++;
        right--;
    }

    // 5. If the loop completes, it's a palindrome
    return true;
};
```
```js
    // Alternative concise approach:
var isPalindromeConcise = function(s) {
    const cleaned = s.toLowerCase().replace(/[^a-z0-9]/g, '');
    return cleaned === cleaned.split('').reverse().join('');
};

```

## Related To
- [[data structures/Arrays]]
