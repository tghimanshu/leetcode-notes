---
id: 3054-type-of-triangle
aliases: []
tags: []
---

---

# 3054. Type of Triangle

---

**Difficulty**: Easy
**Date**: 2026-01-17
**url**: https://leetcode.com/problems/type-of-triangle/
**tags**: [leetcode]

---

## Problem Statement

https://leetcode.com/problems/type-of-triangle/

## 🧠 Idea (1–2 sentences)

- determine the type of triangle based on the sides
- return `equilateral` if all sides are equal, `isosceles` if exactly two sides are equal, and `scalene` if all sides are different.

## 🔧 Approach

- Compare the three sides of the triangle.
- Use conditional statements to check for equality among the sides and return the appropriate triangle type.
- First condition is for equilateral triangle
- second condition to ensure the sides for a valid triangle
  - check if any two sides are equal for isosceles triangle
  - else return scalene triangle
- else return none

## 🧪 Edge Cases

- ensure the triangle is valid with given sides
- To check, the sum of any two sides must be greater than the third side.
- It should be true for all three combinations of sides.
- If the sides do not satisfy this condition, return "none".

## ⌚ Complexities

- Time Complexity: O(1)
- Space Complexity: O(1)
