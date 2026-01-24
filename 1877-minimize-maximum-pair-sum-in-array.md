---
id: 1877-minimize-maximum-pair-sum-in-array
aliases: []
tags: []
---

# 1877. Minimize Maximum Pair Sum in Array

---

**Difficulty**: Medium
**Date**: 2026-01-24 (Daily)
**url**: https://leetcode.com/problems/minimize-maximum-pair-sum-in-array
**tags**: [leetcode]

---

## Problem Statement

U need to find the minized pairs sum in the array. Find the Maximum pair sum in the array.

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- Sort the array and pair the smallest and largest elements to minimize the maximum pair sum.
- it works cause pairing extremes minimizes the largest sums.
- This approach ensures that no single pair sum becomes excessively large.
- Now loop through half the array and calculate som of pairs of left and right pointer.
- Keep track of maximum sum and return it.

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Sort the array in ascending order
- initialize `result` to 0
- Loop `i` from 0 to `n / 2` (excluding `n / 2`):
  - Calculate `pair_sum` as `nums[i] + nums[n - 1 - i]`
  - Update `result` to be the maximum of `result` and `pair_sum`

## 🧪 Edge Cases

- The array is always of even length as per problem constraints.
- nums contains only positive integers.

## ⌚ Complexities

- Time Complexity: O(n log n)
- Space Complexity: O(1)
