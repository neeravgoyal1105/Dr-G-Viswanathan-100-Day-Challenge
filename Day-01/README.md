# Day 01 – Max Consecutive Ones

**Platform:** LeetCode

**Problem Number:** 485

**Language:** C++

## Problem Description
Given a binary array `nums`, return the maximum number of consecutive 1s in the array.

## Approach: Linear Traversal

- Initialize `count` and `maxi` to 0.
- Traverse the array.
- If the current element is 1, increment `count`.
- Update `maxi` whenever a new maximum is found.
- If the current element is 0, reset `count` to 0.
- Return `maxi`.

## Complexity Analysis

- **Time Complexity:** O(n) – Single traversal of the array.
- **Space Complexity:** O(1) – Constant extra space.

## Key Learnings
- Array Traversal
- Consecutive Element Counting
- Maximum Value Tracking
- Time and Space Complexity

**Status:** Accepted ✅

**Test Cases:** 45/45 Passed

[LeetCode Problem – Max Consecutive Ones](https://leetcode.com/problems/max-consecutive-ones/)
