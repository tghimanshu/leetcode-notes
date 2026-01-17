---
id: 2535-difference-between-element-sum-and-digit-sum-of-an-array
aliases: []
tags: []
---

---

# 2535. Difference Between Element Sum and Digit Sum of an Array

---

**Difficulty**: Easy
**Date**: 2026-01-17
**url**: https://leetcode.com/problems/difference-between-element-sum-and-digit-sum-of-an-array/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/difference-between-element-sum-and-digit-sum-of-an-array/

## 🧠 Idea (1–2 sentences)

- we need to find absolute diff between nuumber vs digits of numbers sum in array
- since if a number is single digit, it's digit sum is the number itself, so we can just skip them.
- loop and calculate both sums and return absolute difference
- returt basicn the result

## 🔧 Approach

- setup a `total variable
- loop through all the numbers in the array
- if it's a single digit ignore it
- else add the number to the `total`
- subtract the digits from the `total`
- return the `total` at the end of the loop

## 🧪 Edge Cases

- ensure the number is absolute
- sum of digits is going to be less than or euqal to the number so no need to check for negative values in our approach
- it is taken care automatically by the logic
- to be safe we can use absolute value function

## ⌚ Complexities

- Time Complexity: O(N)
- Space Complexity: O(1)
