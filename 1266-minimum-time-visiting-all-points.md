---
id: 1266-minimum-time-visiting-all-points
aliases: []
tags: []
---

# 1266. Minimum Time Visiting All Points

---

**Difficulty**: Easy
**Date**: 2026-01-12
**url**: https://leetcode.com/problems/minimum-time-visiting-all-points/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/minimum-time-visiting-all-points/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- initial thought was to use euclidean formula but doesn't work cause diagnol is counted as 1 and in euclidean it's counted as 1.14 (sqrt of 2) as it takes more time to travel diagnally
- Second thought was to loop all points then while loop to traverse and get the result but it timed out
- Finally used Chebyshev Distance formula

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Navigate to all the points
- Chebyshev Formula: max(|x2 - x1|, |y2 - y1|) -> where (x1,x2) is first point and (y1, y2) is the second point
- Sum all the values
- Return the sum

## 🧪 Edge Cases

- Unfeasiable idea 1
- TLE (Time limited Exceed) for idea 2

## ⌚ Complexities

- Time Complexity: O(N)
- Space Complexity: O(1)

## Reference

- [https://www.youtube.com/watch?v=xHOt3GGmbvo&t=298s]
