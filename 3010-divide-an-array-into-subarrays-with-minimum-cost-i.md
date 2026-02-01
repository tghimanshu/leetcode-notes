---
id: 3010-divide-an-array-into-subarrays-with-minimum-cost-i
aliases: []
tags: []
---
# 3010. Divide an Array Into Subarrays With Minimum Cost I
---
**Difficulty**: Easy
**Date**: 2026-02-01 (Daily)
**url**: https://leetcode.com/problems/divide-an-array-into-subarrays-with-minimum-cost-i
**tags**: [leetcode]
---
## Problem Statement
we need to divide the array in 3 sub arrays so that we get the min cost
the cost is calculated of first element of each sub array

## 🧠 Idea (1–2 sentences)
<!-- What was the core insight? -->

since we want to minimize cost 
1. we can simply take the first element as it will always the first subarray's first element
2. take 2 min values from the rest of the array and you are done

## 🔧 Approach
<!-- Bullets. No paragraphs. -->

- Initialize variable `total`
- add `nums[0]` to `total`
- Sort the array
- Add `nums[0]` and `nums[1]` to `total`
- return `total`

## 🧪 Edge Cases
- the edge case was when i tried to solve it in bruteforce way and duplicate values created issues

## ⌚ Complexities
- Time Complexity: O(n log n)
- Space Complexity: O(1)
