# 865. Smallest Subtree with all the Deepest Nodes

**Difficulty**: Medium
**Date**: 2026-01-09 (Daily)

## Problem Statement

https://leetcode.com/problems/smallest-subtree-with-all-the-deepest-nodes/

## 🧠 Idea (1–2 sentences)

<!-- What was the core insight? -->

We have a tree and need to find the nodes with depth such that all nodes are covered with the bigger depth

Learnings from the solution used:

- Ensure to understand the question well
- The question states to show the tree with all the deepest nodes
- The failing test case in my code happened cause left goes to depth 3 while right goest to 2
- So only the left tree would be used and right can be skipped and we go till the depth 1 since we need to have all leaf nodes covered

## 🔧 Approach

<!-- Bullets. No paragraphs. -->

Navigate the nodes in dfs (was thinking bfs but didn't knew how to effectively implement/use in this scenario)
Store the nodes in a dict with depth as key having tuple (parent, node)
Loop through the largest to smallest depth
if it's alone return the element
if there are 2 with same parent return the parent
if there are 2 with different parent go to a smaller node and keep comparing

## 🧪 Edge Cases

- Stuck: test case 54 -> can't seem to work correctly
