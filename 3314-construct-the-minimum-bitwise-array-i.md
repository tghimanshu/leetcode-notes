---
id: 3314-construct-the-minimum-bitwise-array-i
aliases: []
tags: []
---

# 3314. Construct the Minimum Bitwise Array I

---

**Difficulty**: Easy
**Date**: 2026-01-20 (Daily)
**url**: https://leetcode.com/problems/construct-the-minimum-bitwise-array-i
**tags**: [leetcode]

---

## Problem Statement

Calculate the smallest possible value satisfying the cnodition `ans[i] or (ans[i] + 1)`
if nothing matches we give ans[i] as `-1`

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- for every number we can just run a forloop for 0 to that number and see if this condition satisfies
- if we find none we will return -1 for that number

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- go through all the numbers
  - go through 0 to number (inclusive)
    - do bit calculation `i or (i + 1)` in code it will be `i | (i + 1)` -> here `|` is for bitwise OR calculation
  - if no number matched answer is -1
- return the answer array

## 🧪 Edge Cases

- if no number matches it should result -1

## ⌚ Complexities

- Time Complexity: O(nums \* n)
- Space Complexity: O(n)
