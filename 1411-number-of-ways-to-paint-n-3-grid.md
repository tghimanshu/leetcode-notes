# 1411. Number of Ways to Paint N × 3 Grid

**Difficulty**: Hard
**Date**: 2026-01-03 (Daily)

## Problem Statement

https://leetcode.com/problems/number-of-ways-to-paint-n-3-grid/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

We have 2 types of color combinations (2 colors) or (3 Colors)
(Red, Yellow, Green) as ABC
SO,
2 Colors: ABA, ACA, BAB, BCB, CAC, CBC -> 6 Possible Combinations
3 Colors: ABC, BCA, CAB, BAC, ACB, CBA -> 6 Possible Combinations
For the first Row -> 6 + 6 = 12 Combinations

For Row 2,
We have to eliminate a set of values depending on the one we select as we cannot have 2 adjacent colors
2 Colors: ABA (is the selection can be any of the 6)

    Selection       -> ABA, ABA, ABA
    Possible ABA's  -> BAB, BCB, CAC  -> only 3 possibilites for every possible one
    Selection       -> ABA, ABA
    Possible ABC's  -> CAB, BAC -> Only 2 Possible Combinations

    Means, for every ABA, we have 3 ABA's and 2 ABC's

Similarly,
3 Colors: ABC (is the selection can be any of the 6)

    Selection       -> ABC, ABC, ABC
    Possible ABA's  -> BAB, BCB -> only 2 possibilites for every possible one
    Selection       -> ABC, ABC
    Possible ABC's  -> BCA, CAB -> Only 2 Possible Combinations

    Means, for every ABC, we have 2 ABA's and 2 ABC's

That's why, For Row 2
6 ABA's -> (6 \* (ABC)) + (6 \* (ABA)) = (6 \* 2) + (6 \* 3) = 12 + 18 = 30
6 ABC's -> (6 \* (ABC)) + (6 \* (ABA)) = (6 \* 2) + (6 \* 2) = 12 + 12 = 24
= 54

Also now we know that we will have 30 ABAs and 24 ABCs
so
30 ABA's -> (30 \* (ABC)) + (30 \* (ABA)) = (30 \* 2) + (30 \* 3) = 60 + 90 = 150
24 ABC's -> (24 \* (ABC)) + (24 \* (ABA)) = (24 \* 2) + (24 \* 2) = 48 + 48 = 096
= 246

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

- get initial row 1 values
- Start looping through all the values and calculate the answers
- Update the inital values and continue till the (N) is reached

## 🧪 Edge Cases

- Could mess up if we don't remember to look at all possibilites individually

## Complexities

- Time Complexity: O(N)
- Spacae Complexity: O(1)
