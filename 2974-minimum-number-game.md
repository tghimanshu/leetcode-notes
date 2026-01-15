---
id: 2974-minimum-number-game
aliases: []
tags: []
---

# 2974. Minimum Number Game

---

**Difficulty**: Easy
**Date**: 2026-01-15
**url**: https://leetcode.com/problems/minimum-number-game/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/minimum-number-game/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- alice takes the min bob takes the second min and then bobs places it first than alice does
- so the result is technically sorted but every 2 elements are swapped

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- sort the array
- swap 2 numbers while stepping 2 steps forward

-

## 🧪 Edge Cases

- no notable edge case as question does mention it's always going to be an even length input array

## ⌚ Complexities

- Time Complexity: O(N^2) -> Used bubble sort but can be reduced by using quicksort or merge sort
- Space Complexity: O(1) -> doing everything in place
