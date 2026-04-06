# Generate Parentheses
Difficulty: **Medium**

**The Scenario:** You are creating a **Code Linter for a Custom Markup Language**. The language requires every "Open Tag" `<` to be eventually closed by a "Close Tag" `>`. You need to provide a "Template Autocomplete" feature that shows all possible valid, balanced configurations of $N$ pairs of tags.

- **The Goal:** Generate all mathematically valid combinations of $N$ opening and closing tags.

## Requirements
- Given `n` pairs of parentheses, write a function to generate all combinations of well-formed parentheses.
- 1 <= n <= 8

## Test Cases
```js
generateParenthesis(3) // ["((()))","(()())","(())()","()(())","()()()"]
generateParenthesis(1) // ["()"]
```

## Solution

```ts
function generateParenthesis(n: number): string[] {
    const result: string[] = [];

    function backtrack(currentString: string, openCount: number, closeCount: number) {
        // Base case: If current string length is 2*n, we have a valid combination
        if (currentString.length === 2 * n) {
            result.push(currentString);
            return;
        }

        // If we can add an open parenthesis, do it
        if (openCount < n) {
            backtrack(currentString + "(", openCount + 1, closeCount);
        }

        // If we can add a close parenthesis (must be less than open count to be valid), do it
        if (closeCount < openCount) {
            backtrack(currentString + ")", openCount, closeCount + 1);
        }
    }

    backtrack("", 0, 0);
    return result;
}
```

## Related To
- [[data structures/Stack]]
