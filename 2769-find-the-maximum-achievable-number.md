---
id: 2769-find-the-maximum-achievable-number
aliases: []
tags: []
---

# 2769. Find the Maximum Achievable Number

---

**Difficulty**: Easy
**Date**: 2026-01-14
**url**: https://leetcode.com/problems/find-the-maximum-achievable-number/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/find-the-maximum-achievable-number/

## 🧠 Idea (1–2 sentences)

- lets imagine `x` is the max achievable number
- from num to x we can go by incrementing num and decrementing x
- so num + t = x - t (cause we have to do the operation t times)
  - Note: We don't need to increment most achievable number cause we go away from num
  - similar we can't decrement num cause we are going away from x
- So, num + t + t = x
- num + 2t = x

## 🔧 Approach

- So just do num + 2t

## 🧪 Edge Cases

- Ensure the constraints doesn't have negative (t)

## ⌚ Complexities

- Time Complexity: O(1)
- Space Complexity: O(1)
