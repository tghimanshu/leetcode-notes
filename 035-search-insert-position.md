---
id: 035-search-insert-position
aliases: []
tags: []
---

# 35. Search Insert Position

---

**Difficulty**: Easy
**Date**: 2026-01-14
**url**: https://leetcode.com/problems/search-insert-position/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/search-insert-position/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- since we know log n is the required time complexity it's simply a binary search problem
- so we do the binary search if we find the target we print the index
- else we can just print the high number (which will be same as low when 0 values are left)
- that is the index where we would need to add the target value

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- perform a binary search
- check for target
- check if num is smaller
- check if num is larger
- if ntg matches print the high value

## 🧪 Edge Cases

- I was using `(low + (high - low)) // 2` causing a TLE
- Issue was that i need to do division first so `low + (high - low) // 2` is the right way
- Additionally, u can just do `(low + high) // 2`
- This was faced while 2nd and 3rd test case

## ⌚ Complexities

- Time Complexity: O(log N)
- Space Complexity: O(1)
