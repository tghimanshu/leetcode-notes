---
id: 042-trapping-rain-water
aliases: []
tags: []
---

# 42. Trapping Rain Water

---

**Difficulty**: Hard
**Date**: 2026-01-28
**url**: https://leetcode.com/problems/trapping-rain-water/
**tags**: [leetcode]

---

## Problem Statement

we need to find how much water can be trapped after raining given the array of pillar heights.

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

- start at 0
- track trappable space
- curr pointer from 0 till same or bigger is found
- if a bigger or equal pointer is found
  - calculate the trapped water
  - make the start as the current
  - start traversing curr forward
- if curr is at end and start not at end
  - move start one space forward
  - if it's end return
  - if it's not
  - make current = start
  - continue tracking trappable water
  - once with this start is at end
  - return the final result

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Pseudo Code
- start = 0
- end = len(input)
- trappable_space = []
- curr = 0
- total_water = 0
- while curr != end:
  - if input[start] <= input[curr]:
    - total += len(trappable_wter) \* min(input[start], input[curr]) - sum(trappable_space)
    - start = curr
    - trappable_space = []
    - continue

  - trappable_space += input[curr]
  - curr += 1

- reverse the pending elements append the start elemnt to the reversed array
- redo the while loop for the reversed array

## 🧪 Edge Cases

- If there a pillar with the max height in between everything after it doesn't get counted
  - addressed by reversing the remaining elements then appending the highest pillar to the end of the reversed array
  - then redoing the same logic

## ⌚ Complexities

- Time Complexity: O(N^2)
- Space Complexity: O(N)
