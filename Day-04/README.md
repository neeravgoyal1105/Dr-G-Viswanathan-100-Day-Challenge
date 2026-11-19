# Day 04 – Remove Duplicates from Sorted Array

**Platform:** LeetCode  
**Problem Number:** 26  
**Language:** C++

## Problem Description

Given an integer array `nums` sorted in non-decreasing order, remove the duplicates in-place so that each unique element appears only once.

Return the number of unique elements (`k`).

The relative order of the elements should be maintained.

## Approach Used: Two Pointer Technique

I solved this problem using the Two Pointer approach.

1. Initialize `i = 0` to track the position of the last unique element.
2. Start traversing the array using `j` from index `1`.
3. If `nums[i]` is not equal to `nums[j]`, update `nums[i+1]` with `nums[j]` and increment `i`.
4. If both elements are equal, skip the duplicate.
5. Finally, return `i + 1` as the count of unique elements.

## Complexity Analysis

- **Time Complexity:** O(n) – Traversing the array once.
- **Space Complexity:** O(1) – Using constant extra space.

## Key Learnings

- Understanding the Two Pointer Technique.
- Removing duplicates from a sorted array.
- In-place array modification.
- Efficient array traversal.
- Maintaining unique elements without using extra space.

## Submission Status

- **Status:** Accepted
- **Test Cases Passed:** 362/362
- **Runtime:** 0 ms (Beats 100.00%)
- **Memory:** 22.77 MB

Successfully solved LeetCode Problem 26 using C++ and the Two Pointer technique.
