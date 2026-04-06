# Binary Tree Level Order Traversal
Difficulty: **Medium**

**The Scenario:** You are building an **Organizational Chart Visualizer** for a massive corporation. The CEO is at the root, and each manager has subordinates. The UI needs to render the staff "level by level" (all VPs first, then all Directors, then all Managers) to ensure the layout remains balanced on the screen.

- **The Goal:** Group all employees by their "distance" from the CEO and return them as a list of levels.

## Requirements
- Given the `root` of a binary tree, return the level order traversal of its nodes' values. (i.e., from left to right, level by level).

## Test Cases
```js
// Tree: [3,9,20,null,null,15,7]
levelOrder(root) // returns [[3],[9,20],[15,7]]

// Tree: [1]
levelOrder(root) // returns [[1]]

// Tree: []
levelOrder(root) // returns []
```

## Solution

```ts
class TreeNode {
    val: number
    left: TreeNode | null
    right: TreeNode | null
    constructor(val?: number, left?: TreeNode | null, right?: TreeNode | null) {
        this.val = (val === undefined ? 0 : val)
        this.left = (left === undefined ? null : left)
        this.right = (right === undefined ? null : right)
    }
}

function levelOrder(root: TreeNode | null): number[][] {
    if (!root) return [];

    const levels: number[][] = [];
    const queue: TreeNode[] = [root];

    while (queue.length > 0) {
        const levelSize = queue.length;
        const currentLevel: number[] = [];

        for (let i = 0; i < levelSize; i++) {
            const node = queue.shift()!;
            currentLevel.push(node.val);

            if (node.left) queue.push(node.left);
            if (node.right) queue.push(node.right);
        }

        levels.push(currentLevel);
    }

    return levels;
}
```

## Related To
- [[data structures/Queue]]
- [[data structures/Binary Search Tree]]
