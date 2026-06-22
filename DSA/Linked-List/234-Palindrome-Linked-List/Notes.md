# 234. Palindrome Linked List

## Problem

Given the head of a linked list.

Return true if it is a palindrome.
Otherwise return false.

---

## Example 1

Input:
1 -> 2 -> 2 -> 1

Output:
True

---

## Example 2

Input:
1 -> 2

Output:
False

---

## Approach

1. Traverse the linked list.
2. Store all values in an array.
3. Compare array with its reverse.
4. If equal → palindrome.
5. Otherwise → not palindrome.

---

## Trick

Python provides reverse slicing:

arr[::-1]

This gives reversed array in one line.

---

## Dry Run

List:

1 -> 2 -> 2 -> 1

Array:

[1,2,2,1]

Reverse:

[1,2,2,1]

Equal

Return True

---

## Time Complexity

O(n)

---

## Space Complexity

O(n)

Array stores all node values.

---

## Interview Follow-up

Can you solve it in O(1) extra space?

Yes.

Using:
- Fast & Slow Pointer
- Reverse Second Half
- Compare Both Halves

This is the optimized interview solution.
