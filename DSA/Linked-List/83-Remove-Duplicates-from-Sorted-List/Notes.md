# 83. Remove Duplicates from Sorted List

## Problem

Given the head of a sorted linked list.

Delete all duplicates such that each element appears only once.

Return the linked list sorted as well.

---

## Example

Input:
head = [1,1,2]

Output:
[1,2]

Input:
head = [1,1,2,3,3]

Output:
[1,2,3]

---

## Approach

1. Start from head.
2. Compare current node with next node.
3. If values are same:
   - Skip next node.
4. Otherwise:
   - Move current forward.
5. Continue until list ends.

---

## Trick

Since the list is already sorted, duplicates will always be adjacent.

No need for HashSet or extra space.

---

## Dry Run

1 -> 1 -> 2 -> 3 -> 3

Current = 1

1 == 1

Remove duplicate

1 -> 2 -> 3 -> 3

Move ahead

3 == 3

Remove duplicate

1 -> 2 -> 3

Done

---

## Time Complexity

O(n)

---

## Space Complexity

O(1)

---

## Interview Question

Why doesn't this work for an unsorted linked list?

Because duplicates won't necessarily be adjacent.
For unsorted lists, extra memory (HashSet) is usually required.
