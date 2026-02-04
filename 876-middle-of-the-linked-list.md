---
id: 876-middle-of-the-linked-list
aliases: []
tags: []
---

# 876. Middle of the Linked List

---

**Difficulty**: Easy
**Date**: 2026-02-04
**url**: https://leetcode.com/problems/middle-of-the-linked-list/
**tags**: [leetcode]

---

## Problem Statement

find the middle note of the linked list.

A great question to learn slow and fast pointer technique.

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- have 2 pointers slow and fast
- slow moves 1 step at a time (head.next)
- fast moves 2 steps at a time (head.next.next)
- when fast reaches the end (where fast and fast.next is valid but fast.next.next is null)
- slow is at the middle node
- if it's an even length list, slow will be on the second middle node

## 🧪 Edge Cases

- list with only 1 node

## ⌚ Complexities

- Time Complexity: O(n)
- Space Complexity: O(1)
