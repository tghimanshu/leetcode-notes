# 1975. Maximum Matrix Sum

**Difficulty**: Medium
**Date**: 2026-01-05 (Daily)

## Problem Statement

https://leetcode.com/problems/maximum-matrix-sum/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

You have to multiply two numbers by -1 aonce and increase the total

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- As you know you can keep swapping till 2 negatives are adjacent and then swap to positive
- When the entire matrix can have one pending -1 which cannot be turned positive
- To ensure the highest sum we make the smallest number in the matrix negative (0 if 0 is the smallest)
- Done

## 🧪 Edge Cases

- We have to take total of absolutes
- Count the number of negatives
- If negatives are even just display total (cause all can be turned positive)
- If negatives are odd we have to subtract double of the lowest value (cause we have added it so we have to remove it once and then subtract it again to ensure it's actually being negative (minimum negative value \* 2))
  - This Ensures that the total is of all the values minus the pending negative value

## Complexities

- Time Complexity: O(N^2)
- Space Complexity: O(1)
