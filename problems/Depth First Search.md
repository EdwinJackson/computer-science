# Number of Islands
Difficulty: **Medium**

**The Scenario:** You are working on **Satellite Imaging Software** for an environmental agency. You have a 2D grid representing a top-down view of a nature reserve where `1` represents dense forest and `0` represents cleared land.

- **The Goal:** Calculate the total number of distinct, isolated forest "clusters" (connected horizontally or vertically) to help ecologists track habitat fragmentation.

## Requirements
- Given an `m x n` 2D binary grid `grid` which represents a map of '1's (land) and '0's (water), return the number of islands.
- An island is surrounded by water and is formed by connecting adjacent lands horizontally or vertically. You may assume all four edges of the grid are all surrounded by water.

## Test Cases
```js
numIslands([
  ["1","1","1","1","0"],
  ["1","1","0","1","0"],
  ["1","1","0","0","0"],
  ["0","0","0","0","0"]
]) // returns 1

numIslands([
  ["1","1","0","0","0"],
  ["1","1","0","0","0"],
  ["0","0","1","0","0"],
  ["0","0","0","1","1"]
]) // returns 3
```

## Solution

```ts
function numIslands(grid: string[][]): number {
    if (!grid || grid.length === 0) return 0;

    let count = 0;
    const rows = grid.length;
    const cols = grid[0].length;

    // DFS helper function to mark visited land
    function dfs(r: number, c: number) {
        if (r < 0 || c < 0 || r >= rows || c >= cols || grid[r][c] === "0") {
            return;
        }

        grid[r][c] = "0"; // Mark as visited (sink the island)

        // Visit all adjacent cells
        dfs(r + 1, c);
        dfs(r - 1, c);
        dfs(r, c + 1);
        dfs(r, c - 1);
    }

    for (let r = 0; r < rows; r++) {
        for (let c = 0; c < cols; c++) {
            if (grid[r][c] === "1") {
                count++;
                dfs(r, c); // Start DFS to find the whole island
            }
        }
    }

    return count;
}
```

## Related To
- [[data structures/Graph]]
- [[data structures/Stack]]
- [[data structures/Arrays]]
