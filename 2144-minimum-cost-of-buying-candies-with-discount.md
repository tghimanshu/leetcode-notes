---
id: 1200-minimum-absolute-difference
aliases: []
tags: []
---

# 2144. Minimum Cost Of Buying Candies With Discount

---

**Difficulty**: Easy
**Date**: 2026-01-26
**url**: https://leetcode.com/problems/minimum-cost-of-buying-candies-with-discount
**tags**: [leetcode]

---

## Problem Statement

Given an array of prices, you can buy 2 and get the 3rd one for free (the price of the cheaper one of 2 bought).
Return the minimum cost to buy all candies.

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- sort the array
- iterate from the most expensive to the cheapest
- for every 3rd candy, skip adding it's price as it's free
- return the total cost

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Sort the array of prices in ascending order.
- Initialize variable `total` to 0.
- Iterate from the end to the start of array:
  - For each index `i`, if `(n - i) % 3 == 0`, skip adding the price (it's free).
  - Otherwise, add the price to `total`.
- Return the `total` cost.

## 🧪 Edge Cases

- only one or 2 candies but since we are using mod 3 it will work fine

## ⌚ Complexities

- Time Complexity: O(n log n)
- Space Complexity: O(1)
