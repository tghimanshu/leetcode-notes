---
id: 1339-maximum-product-of-splitted-binary-tree
aliases: []
tags: []
---

# 1339. Maximum Product of Splitted Binary Tree

---

**Difficulty**: Medium
**Date**: 2026-01-07 (Daily)
**url**: https://leetcode.com/problems/maximum-product-of-splitted-binary-tree/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/maximum-product-of-splitted-binary-tree/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

It is a binary tree and want to calculate products of sum of subtrees.
So using Depth First Search for every node to find the product and compare to the result

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Calculate sum of the tree
- traverse all the nodes and split on that node into 2 subtrees and perform dfs
- Calculate product using the subtree dfs and (total sum - subtree)
- Find the max between result and product of subtrees

## 🧪 Edge Cases

- Time limit exceeded when running with 3 comparisions in the split tree

## ⌚ Complexities

- Time Complexity: O(N)
- Space Complexity: O(H) -> Not sure what this is
