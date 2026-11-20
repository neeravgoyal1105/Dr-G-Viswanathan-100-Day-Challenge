# Day 05 – Missing Number

**Platform:** LeetCode  
**Problem Number:** 268  
**Language:** C++

## Problem Description

Given an array `nums` containing `n` distinct numbers in the range `[0, n]`, return the only number in the range that is missing from the array.

## Approach Used: Mathematical Sum Formula

I solved this problem using the mathematical sum formula.

1. Calculate the expected sum of numbers from `0` to `n` using the formula:

   `sum1 = n * (n + 1) / 2`

2. Initialize `sum2 = 0` to calculate the actual sum of array elements.
3. Traverse the array and add each element to `sum2`.
4. Subtract the actual sum from the expected sum.
5. The result gives the missing number.

**Final Answer:** `sum1 - sum2`

## Complexity Analysis

- **Time Complexity:** O(n) – Traversing the array once.
- **Space Complexity:** O(1) – Using constant extra space.

## Key Learnings

- Understanding the Mathematical Sum Formula.
- Efficient Array Traversal.
- Finding Missing Elements.
- Applying Mathematical Concepts to DSA Problems.
- Optimizing Time and Space Complexity.

## Submission Status

- **Status:** Accepted
- **Test Cases Passed:** 122/122
- **Runtime:** 0 ms (Beats 100.00%)
- **Memory:** 21.61 MB (Beats 85.85%)

Successfully solved LeetCode Problem 268 using C++ and the Mathematical Sum Formula.
