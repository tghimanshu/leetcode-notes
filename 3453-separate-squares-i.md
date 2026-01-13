---
id: 3453-separate-squares-i
aliases: []
tags: []
---

# 3453. Separate Squares I

---

**Difficulty**: Medium
**Date**: 2026-01-13 (Daily)
**url**: https://leetcode.com/problems/separate-squares-i/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/separate-squares-i/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- You have to find area of all the squares and then keep dividing it to get the ideal split
- inital thought was to define a split but best is to use binary search

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- calculate the total area
- get the half way of the area
- set low as lowest square's bottom y and high as highest square's top y
- now calculate the mid of it and find the area for that split
- if the area is bigger reduce the high else reduce the low

## 🧪 Edge Cases

- we need to have a precision factor so we run the code for a certain amount of time in our case 100

## ⌚ Complexities

- Time Complexity: O(N\*K) where
  - n is the input array while
  - k being the constant tries for the precision we are doing which is 100 in our case
- Space Complexity: O(1) just storing over all areas
