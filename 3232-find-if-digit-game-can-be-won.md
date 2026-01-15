---
id: 3232-find-if-digit-game-can-be-won
aliases: []
tags: []
---

# 3232. Find if Digit Game Can Be Won

---

**Difficulty**: Easy
**Date**: 2026-01-15
**url**: https://leetcode.com/problems/find-if-digit-game-can-be-won/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/find-if-digit-game-can-be-won/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- get sum of single digit and double digit number
- to win Alice need to select one which is bigger
- so the only way Alice loses is when both are same

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- calculate sum for single digit and double digit
- return true if both are different

## 🧪 Edge Cases

- we are not comparing greater than and less than and using not equal so that if both values are 0/same it works correctly

## ⌚ Complexities

- Time Complexity: O(N)
- Space Complexity: O(1)
