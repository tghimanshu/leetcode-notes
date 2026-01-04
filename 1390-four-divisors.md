# 1390. Four Divisors

**Difficulty**: Medium
**Date**: 2026-01-04 (Daily)

## Problem Statement

https://leetcode.com/problems/four-divisors/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

For every number in the array we need to find how many divisors are there
Only add it to the sum if total divisors are 4

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- Lopp through all the numbers
- Check if number already in the memoized dictionary then just add the sum and move on to the next number
- Calculate the divisors for sqrt of the number
  - If we go beyond 4 divisors we break and move to next number
  - If we got 4 divisors we add it to final sum
  - We add the number to a memoize dictionary with number as key and sum of the divisors as the value
- Return the result

## 🧪 Edge Cases

- ensuring when doing sqrt calcudation i \* i can be the actual number
- That is, i \* i == num. So we check if that's the case we don't add `i` twice
- For all other we add i and num // i (// means floor divison) to get both multiples of num
- Eseentially, removing the need to go till N and only go till `Root of N`

## Complexities

- Time Complexity: O(N(Root M)) -> N being the list of numbers, M being the unique numbers
- Space Complexity: O(N) -> Storing the seen dictory for memoization

## Extras

```python
__import__("atexit").register(lambda: open('display_runtime.txt','w').write('0'))
```

- TODO: Saw this in some codebase in solutions but not sure what it does
