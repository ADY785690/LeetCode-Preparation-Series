# 206. Reverse Linked List

## Difficulty

Easy

## Problem Statement

Given the head of a singly linked list, reverse the list and return the reversed list.

## Example

Input:

1 -> 2 -> 3 -> 4 -> 5

Output:

5 -> 4 -> 3 -> 2 -> 1

## Approach

Use three pointers:

- prev
- curr
- next

Reverse the direction of each node one by one.

## Dry Run

Original List:

1 -> 2 -> 3 -> 4 -> 5

Initial:

prev = None

curr = 1

Iteration 1:

1 -> None

prev = 1

curr = 2

Iteration 2:

2 -> 1 -> None

prev = 2

curr = 3

Iteration 3:

3 -> 2 -> 1 -> None

prev = 3

curr = 4

Continue until curr becomes None.

Final:

5 -> 4 -> 3 -> 2 -> 1

## Python Solution

```python
class Solution:
    def reverseList(self, head):
        prev = None
        curr = head

        while curr:
            nxt = curr.next
            curr.next = prev
            prev = curr
            curr = nxt

        return prev
```

## Time Complexity

O(n)

## Space Complexity

O(1)

## Pattern Used

Linked List Reversal

## Key Idea

Store the next node before changing links.

Reverse the current node's pointer.

Move both pointers forward.

## Similar Questions

- Reverse Linked List II
- Palindrome Linked List
- Reverse Nodes in K Group
- Reorder List

## Interview Trick

Whenever interviewer says:

- Reverse a Linked List
- Reverse a part of Linked List
- Check Palindrome Linked List

Think:

Linked List Reversal Pattern

## Learning Outcome

- Pointer Manipulation
- In-place Reversal
- O(1) Space Optimization
- Linked List Traversal
