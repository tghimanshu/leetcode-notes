---
id: 3507-minimum-pair-removal-to-sort-array-i
aliases: []
tags: []
---

# 3507. Minimum Pair Removal to Sort Array I

---

**Difficulty**: Easy
**Date**: 2026-01-22 (Daily)
**url**: https://leetcode.com/problems/minimum-pair-removal-to-sort-array-i
**tags**: [leetcode]

---

## Problem Statement

- we need to shorten the array with the min sum of 2 adjacent values until it's sorted

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- continue to combine until we get a sorted array
  - loop through all elements
    - find the minSum pair and index of the first index of pair
  - if array is sorted
    - return the count of operations
  - if array is not sorted
    - add to count
    - store sum of pair to the first index
    - delete the second index value

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- set variables `count` to `0` and `isSorted` to `False`
- while we have unsorted array
  - set `isSorted` to `True`, `minIndex` to -1, and `minSum` to `infinity`
    - loop through all the elements in the array
      - if adjacents values are not sorted set `isSorted` to `False`
      - find the sum of adjacent values if it's less than `minSum`
        - set `minIndex` to the current `index` and `minSum` to the sum
    - if the array is sorted
      - return the `count`
    - if it's not sorted
      - increment `count` by `1`
      - make value of `minIndex` elemnent to `minSum`
      - remove the value in index `minIndex + 1`

## 🧪 Edge Cases

- it doesn't care if the starting piece is also sorted if it's sum is min it needs to be combined
- So [1,1, 5, 2, 8] will combine [1, 1] even if only [5, 2] can be done to just get it in 1 combining
- it's cause minSum of [1, 1] is `2` and [5, 2] is `7`
- we need to count the number of combinations we did and not count if it's sorted

## ⌚ Complexities

- Time Complexity: O(N^2)
- Space Complexity: O(1)
