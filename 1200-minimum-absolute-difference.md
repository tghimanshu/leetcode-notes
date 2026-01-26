---
id: 1200-minimum-absolute-difference
aliases: []
tags: []
---

# 1200. Minimum Absolute Difference

---

**Difficulty**: Easy
**Date**: 2026-01-26 (Daily)
**url**: https://leetcode.com/problems/minimum-absolute-difference
**tags**: [leetcode]

---

## Problem Statement

The idea is to find all pairs of elements in a given array of distinct integers that have the minimum absolute difference between them.

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- since the shortest absolute difference would ideally be between two consecutive numbers we can sort the array first
- then find absolute differences between consecutive elements
- keep track of min absolute difference and all pairs that have that difference
- if any smaller difference is found, reset the list of pairs and update the min difference

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Sort the input array
- Initialize `minPairs` as an empty list and `minDiff` as infinity
- Loop through the sorted array from index 0 to end - 1
  - Calculate the absolute difference between the current element and the next element
  - If the difference is less than `minDiff`
    - Update `minDiff` to this new difference
    - Clear `minPairs` and add the current pair to it
  - Else if the difference equals `minDiff`
    - Add the current pair to `minPairs`

## 🧪 Edge Cases

- None to consider so far

## ⌚ Complexities

- Time Complexity: O(n log n)
- Space Complexity: O(n)
