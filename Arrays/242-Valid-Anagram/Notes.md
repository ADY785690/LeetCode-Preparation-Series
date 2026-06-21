# 242. Valid Anagram

## Problem Statement

Given two strings `s` and `t`, return `true` if `t` is an anagram of `s`, and `false` otherwise.

An Anagram is a word formed by rearranging the letters of another word using all original letters exactly once.

---

## Examples

### Example 1

Input:

```text
s = "anagram"
t = "nagaram"
```

Output:

```text
true
```

### Example 2

Input:

```text
s = "rat"
t = "car"
```

Output:

```text
false
```

---

## Approach

If two strings are anagrams:

* They must have the same length.
* Every character must appear the same number of times in both strings.

We can use Python's `Counter` to count character frequencies and compare them.

---

## Solution

```python
from collections import Counter

class Solution:
    def isAnagram(self, s: str, t: str) -> bool:
        return Counter(s) == Counter(t)
```

---

## Dry Run

Input:

```text
s = "anagram"
t = "nagaram"
```

Counter(s):

```text
{
'a':3,
'n':1,
'g':1,
'r':1,
'm':1
}
```

Counter(t):

```text
{
'n':1,
'a':3,
'g':1,
'r':1,
'm':1
}
```

Both are equal → Return True

---

## Time Complexity

```text
O(n)
```

We traverse each string once.

---

## Space Complexity

```text
O(1)
```

Only lowercase English letters are used.

---

## Pattern Used

Frequency Counting (Hash Map)

---

## Similar Problems

* Group Anagrams
* Find All Anagrams in a String
* Ransom Note
* Valid Palindrome

---

## Key Learning

✅ Counter from collections

✅ Frequency counting

✅ Hash Map usage

✅ String manipulation

LeetCode Difficulty: Easy
