# Linked List Basics

## What is a Linked List?

A Linked List is a linear data structure where elements are connected using pointers.

Example:

10 → 20 → 30 → 40

Each node contains:

- Data
- Pointer to next node

## Advantages

- Dynamic size
- Efficient insertion and deletion

## Disadvantages

- Extra memory for pointers
- No direct access by index

## Basic Node Structure in Python

```python
class Node:
    def __init__(self, data):
        self.data = data
        self.next = None
```

## Common Interview Questions

1. Reverse Linked List
2. Detect Cycle
3. Find Middle Node
4. Merge Two Sorted Lists
5. Remove Nth Node

## Complexity

Access: O(n)

Insertion: O(1)

Deletion: O(1)
