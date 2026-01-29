---
id: 231-power-of-two
aliases: []
tags: []
---

# 231. Power of Two

---

**Difficulty**: Easy
**Date**: 2026-01-29
**url**: https://leetcode.com/problems/power-of-two/
**tags**: [leetcode]

---

## Problem Statement

find if a number is power of two

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- first approach i tried is log n with base 2 should be a x.0 format float
- which means that log(2)16 = 4.0 -> x.0 -> true
- we find that it's x.0 by modding the result with 1 -> 4.0 % 1 == 0 (as 4.5 % 1 = 5)
- ensure it's greather than 0

- second appraoch from solutions is to do bit manipulation
- doing & (AND) between n and n - 1 should result in 0 bits

10000 -> n -> 16
01111 -> n - 1 -> 15
AND=
00000 -> 0

- also we ensure the number is greather than 0 as negative numbers can't be power of 2 or any number

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Approach 1: n > 0 and log2(n) % 1 == 0
- Approach 2: n > 0 and n & (n - 1) == 0

## 🧪 Edge Cases

- n = 0 -> false
- n < 0 -> false

## ⌚ Complexities

- Time Complexity: O(1)
- Space Complexity: O(1)
