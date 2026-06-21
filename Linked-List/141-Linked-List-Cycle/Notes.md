# 141. Linked List Cycle

## Problem

Determine whether a linked list contains a cycle.

## Example

1 → 2 → 3 → 4
↑     ↓
← ← ←

Output:

True

## Approach

Use Floyd's Cycle Detection Algorithm.

Two pointers:

* Slow moves 1 step
* Fast moves 2 steps

If a cycle exists, they will eventually meet.

## Dry Run

1 → 2 → 3 → 4 → 2

Slow and Fast start at head.

Slow: 1 → 2 → 3

Fast: 1 → 3 → 2

Eventually both meet.

Return True.

## Time Complexity

O(n)

## Space Complexity

O(1)

## Interview Trick

Never use HashSet first in interviews.

Optimal solution:

Slow + Fast Pointer

Also called:

Tortoise and Hare Algorithm.
