---
aliases: []
id: 1822-sign-of-the-product-of-an-array
tags: []
---

# 1822. Sign of the Product of an Array

---

**Difficulty**: Easy
**Date**: 2026-01-16
**url**: [https://leetcode.com/problems/sign-of-the-product-of-an-array/]
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/sign-of-the-product-of-an-array/

## 🧠 Idea (1–2 sentences)

- find the product of all the numbers
- if it's negative return -1 if it's 0 return 0 if it's positive return 1

## 🔧 Approach

- Approach 1
  - Initialize a variable `product` to 1.
  - loop through all the numbers and multiply them to `product`
  - if there is a zero in the array directly return 0 (as the product is 0 regarless of other numbers)
  - now check if product is positive return 1 else return -1
- Approach 2 (Optimized)
  - Initialize a variable `negatives` to 1.
  - loop through all the numbers
  - if there is a zero in the array directly return 0 (as the product is 0 regarless of other numbers)
  - if the number is negative increment `negatives` by 1
  - after the loop if `negatives` is even return 1 else return -1

- **Why does the optimization works?**
  - The Product of two negative numbers is positive.
  - calculating product (\*) is expensive than adding (+)
  - so using negatives instead of product reduces the time complexity

## 🧪 Edge Cases

- we return 0 the moment we see a 0 in the array cause the product will be 0 no matter what other numbers are.

## ⌚ Complexities

- Time Complexity: O(N)
- Space Complexity: O(1)
