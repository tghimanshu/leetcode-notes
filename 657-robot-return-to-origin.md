---
id: 657-robot-return-to-origin
aliases: []
tags: []
---

# 657. Robot Return to Origin

---

**Difficulty**: Easy
**Date**: 2026-01-14
**url**: https://leetcode.com/problems/robot-return-to-origin/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/robot-return-to-origin/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- imagine the origin is (0,0) basically center in a graph plane
- makes it easy to just do y+1 when we go UP and y-1 when we go DOWN
- Similarly, x+1 when we go Right and x-1 when we go left
- Finally, check if x == 0 and y == 0

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- loop through all characters in the string
- U = y + 1, D = y - 1, L = x - 1, R = x + 1

## 🧪 Edge Cases

- make sure we check x and y both at the end are 0

## ⌚ Complexities

- Time Complexity: O(N) -> length of string
- Space Complexity: O(1) -> two integers only
