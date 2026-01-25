---
id: 1984-minimum-difference-between-highest-and-lowest-of-k-scores
aliases: []
tags: []
---

# 1984. Minimum Difference Between Highest and Lowest of K Scores

---

**Difficulty**: Easy
**Date**: 2026-01-25 (Daily)
**url**: https://leetcode.com/problems/minimum-difference-between-highest-and-lowest-of-k-scores
**tags**: [leetcode]

---

## Problem Statement

find the minized score difference between the highest and lowest of k scores from the given array of scores.

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- Sort the scores array.
- Use sliding window of size k to find the min difference.
- keep track of the minimum difference found.
- return the minimum difference.

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Sort the scores array in ascending order.
- initialize the variable `minDiff` to infinity.
- Initialize the variable `first` to 0 and last to `k-1`
- Initialize the variable `first` to `0` and last to `k-1`
- while `last` is less than the length of scores:
  - calculate the difference between scores[last] and scores[first]
  - update `minDiff` if the calculated difference is smaller.
  - increment `first` and `last` by 1.
- return `minDiff`.

## 🧪 Edge Cases

- If scores array has less than k elements, return 0 or handle as per requirements.
- the last and sencond last of array won't work cause k can be smaller than the array length
- it also means that there are other elements whose diffence could be lower than the last and second last elements.
- if k is equal to 1, the minimum difference is always 0.

## ⌚ Complexities

- Time Complexity: O(n log n)
- Space Complexity: O(1)
