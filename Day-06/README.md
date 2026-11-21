# Day 06 – Two Sum

## Problem Details
- **Platform:** LeetCode
- **Problem Number:** 1
- **Language:** C++

## Problem Description
Given an array of integers and a target, return the indices of the two numbers such that they add up to the target.

## Approach Used
**Hashing using unordered_map**

1. Traverse the array.
2. Calculate the required number using `target - nums[i]`.
3. Check whether the required number exists in the map.
4. If found, return the indices of both numbers.
5. Otherwise, store the current number and its index in the map.

## Complexity Analysis
- **Time Complexity:** O(n) average
- **Space Complexity:** O(n)

## Submission Status
- **Accepted:** Yes ✅
- **Test Cases Passed:** 66/66
- **Runtime:** 1 ms
- **Memory:** 14.83 MB

## Key Learnings
- Understanding Hashing
- Using unordered_map in C++
- Efficient element lookup
- Improving problem-solving skills

One problem at a time. One day at a time! 🚀
