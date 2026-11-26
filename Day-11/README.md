# Day 11 – Maximum Product of Three Numbers

## Problem Details
- **Platform:** LeetCode
- **Problem Number:** 628
- **Language:** C++

## Problem Description
Given an integer array, find the maximum product of any three numbers in the array.

## Approach Used
**Sorting**

1. Sort the array in ascending order.
2. Calculate the product of the three largest numbers.
3. Calculate the product of the two smallest numbers and the largest number.
4. Return the maximum of these two products.

## Code
```cpp
class Solution {
public:
    int maximumProduct(vector<int>& nums) {
        int n = nums.size();

        if(n == 3) {
            return nums[0] * nums[1] * nums[2];
        }

        sort(nums.begin(), nums.end());

        int product1 = nums[n - 1] * nums[n - 2] * nums[n - 3];
        int product2 = nums[0] * nums[1] * nums[n - 1];

        return max(product1, product2);
    }
};
```

## Complexity Analysis
- **Time Complexity:** O(n log n)
- **Space Complexity:** O(1) auxiliary space

## Submission Status
- **Accepted:** Yes ✅
- **Test Cases Passed:** 98/98
- **Runtime:** 10 ms
- **Memory:** 31.64 MB

## Key Learnings
- Sorting an array
- Handling negative numbers
- Finding maximum products
- Applying mathematical observations

One problem at a time. One day at a time! 🚀
