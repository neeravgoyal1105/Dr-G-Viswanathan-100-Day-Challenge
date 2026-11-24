# Day 09 – Majority Element

## Problem Details
- **Platform:** LeetCode
- **Problem Number:** 169
- **Language:** C++

## Problem Description
Given an array of size `n`, find the element that appears more than `n/2` times. The majority element is guaranteed to exist.

## Approach Used
**Sorting**

1. Sort the array in ascending order.
2. Calculate the size of the array.
3. Return the element at index `n/2`.
4. Since the majority element appears more than half the time, it will occupy the middle position after sorting.

## Code
```cpp
class Solution {
public:
    int majorityElement(vector<int>& nums) {
        sort(nums.begin(), nums.end());
        int n = nums.size();
        return nums[n/2];
    }
};
```

## Complexity Analysis
- **Time Complexity:** O(n log n)
- **Space Complexity:** O(1) auxiliary space

## Submission Status
- **Accepted:** Yes ✅
- **Test Cases Passed:** 59/59
- **Runtime:** 5 ms
- **Memory:** 42.01 MB

## Key Learnings
- Sorting an array
- Finding the majority element
- Applying mathematical observations
- Understanding time and space complexity

One problem at a time. One day at a time! 🚀
