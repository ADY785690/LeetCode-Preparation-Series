# 876. Middle of the Linked List

## Difficulty
Easy

## Problem Statement

Given the head of a singly linked list, return the middle node of the linked list.

If there are two middle nodes, return the second middle node.

## Example 1

Input:
1 -> 2 -> 3 -> 4 -> 5

Output:
3 -> 4 -> 5

## Example 2

Input:
1 -> 2 -> 3 -> 4 -> 5 -> 6

Output:
4 -> 5 -> 6

## Approach

Use two pointers:

- Slow Pointer
- Fast Pointer

Slow moves one step at a time.

Fast moves two steps at a time.

When Fast reaches the end, Slow will be at the middle.

## Dry Run

Linked List:

1 -> 2 -> 3 -> 4 -> 5

Initial:

Slow = 1
Fast = 1

Move 1:

Slow = 2
Fast = 3

Move 2:

Slow = 3
Fast = 5

Fast reaches end.

Answer = 3

## Python Solution

```python
class Solution:
    def middleNode(self, head):
        slow = head
        fast = head

        while fast and fast.next:
            slow = slow.next
            fast = fast.next.next

        return slow
```

## Time Complexity

O(n)

## Space Complexity

O(1)

## Pattern Used

Fast and Slow Pointer

## Similar Questions

- Linked List Cycle
- Happy Number
- Find Nth Node From End

## Interview Trick

Whenever you see:

- Find Middle Node
- Detect Cycle
- Nth Node From End

Think:

Fast & Slow Pointer
