---
id: 1832-check-if-the-sentence-is-pangram
aliases: []
tags: []
---

# 1832. Check if the Sentence Is Pangram

---

**Difficulty**: Easy
**Date**: 2026-01-29
**url**: https://leetcode.com/problems/check-if-the-sentence-is-pangram/
**tags**: [leetcode]

---

## Problem Statement

- [!] check if a sentence is a pangram, meaning it contains all the letters atleast once.

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- use a set to track unique letters
- check if the size of the set is 26

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- initialize an empty set
- iterate through each character in the sentence and add it to the set
- return true if size is 26, else false

-

## 🧪 Edge Cases

- none

## ⌚ Complexities

- Time Complexity: O(n)
- Space Complexity: O(1)
