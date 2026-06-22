# 21. Merge Two Sorted Lists

## Problem

Given the heads of two sorted linked lists list1 and list2.

Merge the two lists into one sorted linked list and return its head.

---

## Example

Input:
list1 = [1,2,4]
list2 = [1,3,4]

Output:
[1,1,2,3,4,4]

---

## Approach

1. Create a dummy node.
2. Compare nodes from both lists.
3. Attach the smaller node to the merged list.
4. Move the pointer forward.
5. When one list ends, attach the remaining part of the other list.

---

## Trick

Use a dummy node.

This avoids handling special cases for the head node separately.

---

## Time Complexity

O(n + m)

n = length of list1

m = length of list2

---

## Space Complexity

O(1)

Only pointers are used.

---

## Interview Question

Why use a dummy node?

Because it simplifies pointer handling and avoids extra conditions for the first node.
