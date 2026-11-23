# Day 08 – Search Insert Position

## Problem Details
- **Platform:** LeetCode
- **Problem Number:** 35
- **Language:** C++

## Problem Description
Given a sorted array of distinct integers and a target value, return the index if the target is found. If not, return the index where it should be inserted in order.

## Approach Used
**Binary Search**

1. Initialize `low = 0` and `high = n`.
2. Calculate the middle index using `(low + high) / 2`.
3. If `nums[mid] == target`, return `mid`.
4. If `nums[mid] < target`, update `low = mid + 1`.
5. Otherwise, update `high = mid`.
6. Return `low` when the search ends.

## Code
```cpp
class Solution {
public:
    int searchInsert(vector<int>& nums, int target) {
        int n = nums.size();
        int low = 0;
        int high = n;

        while(low < high) {
            int mid = (low + high) / 2;

            if(nums[mid] == target) {
                return mid;
            }
            else if(nums[mid] < target) {
                low = mid + 1;
            }
            else {
                high = mid;
            }
        }

        return low;
    }
};
```

## Complexity Analysis
- **Time Complexity:** O(log n)
- **Space Complexity:** O(1)

## Submission Status
- **Accepted:** Yes ✅
- **Test Cases Passed:** 68/68
- **Runtime:** 0 ms
- **Memory:** 13.69 MB

## Key Learnings
- Binary Search
- Searching in a sorted array
- Understanding search boundaries
- Finding the correct insertion position

One problem at a time. One day at a time! 🚀
