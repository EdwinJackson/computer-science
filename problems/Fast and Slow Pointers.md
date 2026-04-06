# Linked List Cycle
Difficulty: **Easy**

**The Scenario:** You are debugging a **Distributed Task Scheduler**. Each task points to the "Next Task" to be executed. You suspect a "Deadlock Loop" where Task A points to B, B to C, and C points back to A, causing the processor to spin infinitely.

- **The Goal:** Write a memory-efficient diagnostic to determine if the task chain contains a circular dependency without storing every task ID you've already seen.

## Requirements
- Given `head`, the head of a linked list, determine if the linked list has a cycle in it.
- There is a cycle in a linked list if there is some node in the list that can be reached again by continuously following the `next` pointer.
- Return `true` if there is a cycle in the linked list. Otherwise, return `false`.

## Test Cases
```js
// [3,2,0,-4], pos = 1 (tail connects to node index 1)
hasCycle(head) // returns true

// [1,2], pos = 0
hasCycle(head) // returns true

// [1], pos = -1
hasCycle(head) // returns false
```

## Solution

```ts
class ListNode {
    val: number
    next: ListNode | null
    constructor(val?: number, next?: ListNode | null) {
        this.val = (val === undefined ? 0 : val)
        this.next = (next === undefined ? null : next)
    }
}

function hasCycle(head: ListNode | null): boolean {
    if (!head || !head.next) {
        return false;
    }

    let slow: ListNode | null = head;
    let fast: ListNode | null = head.next;

    while (slow !== fast) {
        if (!fast || !fast.next) {
            return false;
        }
        slow = slow!.next;
        fast = fast.next.next;
    }

    return true;
}
```

## Related To
- [[data structures/Linked Lists]]
