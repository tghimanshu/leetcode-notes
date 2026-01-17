---
aliases: []
id: 1550-three-consecutive-odds
tags: []
---

# 1550. Three Consecutive Odds

---

**Difficulty**: Easy
**Date**: 2026-01-17
**url**: https://leetcode.com/problems/three-consecutive-odds/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/three-consecutive-odds/

## 🧠 Idea (1–2 sentences)

- we need to check if there are three consecutive odd numbers in the array
- we can loop through the array and maintain a counter for odd numbers

## 🔧 Approach

- simplest way is to setup a variable named `odds` and set it to zero (0)
- loop through all the numbers in the array
- if the value is odd, increment the `odds` variable by one (1)
- if the incremented value of `odds` is three (3), return true
- if the value is even, reset the value of `odds` to zero (0)
- if loop ends, return false

## 🧪 Edge Cases

- None identified

## ⌚ Complexities

- Time Complexity: O(N)
- Space Complexity: O(1)
