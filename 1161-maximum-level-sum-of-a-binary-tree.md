# 1161. Maximum Level Sum of a Binary Tree

**Difficulty**: Medium
**Date**: 2026-01-06 (Daily)

## Problem Statement

https://leetcode.com/problems/maximum-level-sum-of-a-binary-tree/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

Do a breath first search and calculate the sum and compare with the max
If the sum is max, save the max value and the depth of the tree too

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Do a breath first search
- Calculate Sum
- Compare to the resultSum
  - If the sum is larger, update the resultSum and resultDepthIndex
- Return resultDepthIndex

## 🧪 Edge Cases

-

## Complexities

- Time Complexity: O(N)
- Space Complexity: O(N) -> Not Sure got O(W) on leetcode analyze
