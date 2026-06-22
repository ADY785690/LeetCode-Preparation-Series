# 203. Remove Linked List Elements

## Problem

Given the head of a linked list and an integer val.

Remove all nodes that have Node.val == val.

Return the new head.

---

## Example

Input:
head = [1,2,6,3,4,5,6]
val = 6

Output:
[1,2,3,4,5]

---

## Approach

1. Create a dummy node before head.
2. Traverse the list.
3. If next node contains target value:
   - Skip it.
4. Otherwise move ahead.
5. Return dummy.next.

---

## Trick

Use a dummy node.

If the first node itself has to be deleted,
dummy node handles it easily.

---

## Dry Run

1 -> 2 -> 6 -> 3 -> 4 -> 5 -> 6

Target = 6

Remove first 6

1 -> 2 -> 3 -> 4 -> 5 -> 6

Remove last 6

1 -> 2 -> 3 -> 4 -> 5

Done

---

## Time Complexity

O(n)

---

## Space Complexity

O(1)

---

## Interview Question

Why use a dummy node?

Because head itself may need to be removed.
Without dummy node, extra conditions are required.
