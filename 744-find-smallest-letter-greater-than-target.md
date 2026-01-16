---
id: 744-find-smallest-letter-greater-than-target
aliases: []
tags: []
---

---

# 744. Find Smallest Letter Greater Than Target

---

**Difficulty**: Easy
**Date**: 2026-01-16
**url**: https://leetcode.com/problems/find-smallest-letter-greater-than-target/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/find-smallest-letter-greater-than-target/

## 🧠 Idea (1–2 sentences)

- we need to find the next letter greater than target
- inital thought was to do binary search but since the array is small we can just do linear search
- we return the first letter if the last letter is smaller or equal to target (it's an edge case)
- we loop till we find greater letter than target and return it

## 🔧 Approach

- ensure the edge case is handled
- loop through the letters and return the letter which is greater than target

## 🧪 Edge Cases

- we return the first letter if the last letter is smaller or equal to target (it's an edge case)

## ⌚ Complexities

- Time Complexity: O(N)
- Space Complexity: O(1)
