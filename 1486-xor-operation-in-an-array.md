---
id: 1486-xor-operation-in-an-array
aliases: []
tags: []
---

# 1486. XOR Operation in an Array

---

**Difficulty**: Easy
**Date**: 2026-01-14
**url**: https://leetcode.com/problems/xor-operation-in-an-array/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/xor-operation-in-an-array/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- XOR a set of numbers

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- since we know how to create the nums array and have a formula
- create the array runtime and instead of storing the array just do the XOR of the value and store the result

## 🧪 Edge Cases

- Ensure don't add brackets everywhere i was using `(start + 2) * i`
- it clearly stated that it's `start + 2 * i` which means my brackets changed the values making it wrong
- So see when to use brackets
- don't assume that u need brackets when it doesn't, lol!

## ⌚ Complexities

- Time Complexity: O(N)
- Space Complexity: O(1) -> not saving the array just the updating the result while looping through the values
