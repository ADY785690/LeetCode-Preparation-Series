# 876. Middle Of The Linked List

## Problem

Return the middle node of a linked list.

If there are two middle nodes, return the second one.

## Example

Input:

1 → 2 → 3 → 4 → 5

Output:

3

## Approach

Use Slow and Fast pointers.

* Slow moves 1 step.
* Fast moves 2 steps.

When fast reaches the end, slow reaches the middle.

## Dry Run

1 → 2 → 3 → 4 → 5

Slow = 1
Fast = 1

After first move:

Slow = 2
Fast = 3

After second move:

Slow = 3
Fast = 5

Answer = 3

## Time Complexity

O(n)

## Space Complexity

O(1)

## Interview Trick

Remember:

Fast = Fast.next.next

Slow = Slow.next

This pattern is used in many Linked List problems.
