---
id: 3289-the-two-sneaky-numbers-of-digitville
aliases: []
tags: []
---
# 3289. The Two Sneaky Numbers of Digitville
---
**Difficulty**: Easy
**Date**: 2026-02-01
**url**: https://leetcode.com/problems/the-two-sneaky-numbers-of-digitville/
**tags**: [leetcode]
---
## Problem Statement
find the 2 duplicate numbers

## 🧠 Idea (1–2 sentences)
<!-- What was the core insight? -->

- track seen elements
- if the value is in seen array append to result
- if the res is of length 2
    - return res

## 🔧 Approach
<!-- Bullets. No paragraphs. -->

- initialize variable `seen` and `res` as blank arrays
- iterate through all the values
- if value is in seen 
    - append it to `res`
    - if lenght of `res` is `2` return `res`
- else append value to seen

## 🧪 Edge Cases
- None

## ⌚ Complexities
- Time Complexity: O(n)
- Space Complexity: O(n)
