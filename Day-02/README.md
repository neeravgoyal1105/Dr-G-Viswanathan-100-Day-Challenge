
# Day 02 – Rotate Array

**Platform:** LeetCode

**Problem Number:** 189

**Language:** C++

## Problem Description

Given an integer array `nums`, rotate the array to the right by `k` steps, where `k` is non-negative.

## Approach Used: Reversal Algorithm

The array is rotated using three reverse operations:

1. Reverse the entire array.
2. Reverse the first `k` elements.
3. Reverse the remaining elements.

To handle cases where `k` is greater than the array size, use:

`k = k % n`

## Complexity Analysis

- **Time Complexity:** O(n)
- **Space Complexity:** O(1)

## Key Learnings

- Array Manipulation
- Reversal Algorithm
- Two-Pointer Technique
- In-place Operations
- Modulo Operation

## Submission Status

Accepted – 695/695 test cases passed.
