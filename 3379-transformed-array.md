---
id: 3379-transformed-array
aliases: []
tags: []
---

# 3379. Transformed Array

---

**Difficulty**: Easy
**Date**: 2026-02-05 (Daily)
**url**: https://leetcode.com/problems/transformed-array
**tags**: [leetcode]

---

## Problem Statement

transform the array by applying the given conditions

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- If nums[i] > 0: Start at index i and move nums[i] steps to the right in the circular array. Set result[i] to the value of the index where you land.
- If nums[i] < 0: Start at index i and move abs(nums[i]) steps to the left in the circular array. Set result[i] to the value of the index where you land.
- If nums[i] == 0: Set result[i] to nums[i].

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- initialize the result array
- iterate through the input array
- for each element, apply the conditions determined (use modulo since it's a circular array)
- return the result array

## 🧪 Edge Cases

- Array is circular, so we need to use modulo to wrap around the indices.

## ⌚ Complexities

- Time Complexity: O(n)
- Space Complexity: O(n)
