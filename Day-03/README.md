
# Day 03 – Move Zeroes

**Platform:** LeetCode

**Problem Number:** 283

**Language:** C++

## Problem Description

Given an integer array `nums`, move all `0's` to the end of it while maintaining the relative order of the non-zero elements.

You must do this in-place without making a copy of the array.

## Approach Used: Two Pointer Technique

The solution uses a two-pointer approach:

1. Find the index of the first zero in the array.
2. If no zero exists, return.
3. Traverse the remaining array.
4. Whenever a non-zero element is found, swap it with the element at index `j`.
5. Increment `j` after every swap.

This moves all zeroes to the end while maintaining the relative order of non-zero elements.

## Complexity Analysis

- **Time Complexity:** O(n) – The array is traversed linearly.
- **Space Complexity:** O(1) – All operations are performed in-place.

## Key Learnings

- Two Pointer Technique
- Array Manipulation
- In-place Operations
- Swapping Elements
- Maintaining Relative Order

## Submission Status

- **Status:** Accepted
- **Test Cases Passed:** 75/75
- **Runtime:** 0 ms
- **Memory:** 23.69 MB

