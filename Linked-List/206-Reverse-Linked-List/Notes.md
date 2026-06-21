# 206. Reverse Linked List

## Problem

Reverse a singly linked list and return the new head.

## Example

Input:
1 → 2 → 3 → 4 → 5

Output:
5 → 4 → 3 → 2 → 1

## Approach

Use three pointers:

* prev = Previous node
* curr = Current node
* nxt = Next node

Reverse the link one node at a time.

## Dry Run

Original:

1 → 2 → 3

Step 1:
1 ← None

Step 2:
2 ← 1

Step 3:
3 ← 2 ← 1

Return 3

## Time Complexity

O(n)

## Space Complexity

O(1)

## Interview Trick

Always save next node before changing links:

nxt = curr.next

Otherwise remaining list will be lost.
