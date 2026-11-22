# Day 07 – Contains Duplicate

## Problem Details
- **Platform:** LeetCode
- **Problem Number:** 217
- **Language:** C++

## Problem Description
Given an integer array, return `true` if any value appears at least twice, and return `false` if every element is distinct.

## Approach Used
**Sorting**

1. Sort the array in ascending order.
2. Traverse the array.
3. Compare each element with the next element.
4. If two adjacent elements are equal, return `true`.
5. If no duplicates are found, return `false`.

## Code
```cpp
class Solution {
public:
    bool containsDuplicate(vector<int>& nums) {
        sort(nums.begin(), nums.end());

        for(int i = 0; i < nums.size() - 1; i++) {
            if(nums[i] == nums[i + 1]) {
                return true;
            }
        }

        return false;
    }
};
```

## Complexity Analysis
- **Time Complexity:** O(n log n)
- **Space Complexity:** O(1) auxiliary space

## Submission Status
- **Accepted:** Yes ✅
- **Test Cases Passed:** 80/80
- **Runtime:** 29 ms
- **Memory:** 83.36 MB

## Key Learnings
- Sorting an array
- Comparing adjacent elements
- Detecting duplicate values
- Understanding time and space complexity

One problem at a time. One day at a time! 🚀
