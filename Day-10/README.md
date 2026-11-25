# Day 10 – Reverse Integer

## Problem Details

- **Platform:** LeetCode
- **Problem Number:** 7
- **Language:** C++

## Problem Description

Given a signed 32-bit integer, reverse its digits. If the reversed integer goes outside the signed 32-bit integer range, return `0`.

## Approach Used

**Digit Extraction and Reversal**

1. Initialize `rev = 0`.
2. Extract the last digit using `x % 10`.
3. Check for integer overflow before updating `rev`.
4. Add the extracted digit to the reversed number.
5. Remove the last digit from `x` using `x / 10`.
6. Repeat until `x` becomes 0.
7. Return the reversed integer.

## Code

```cpp
class Solution {
public:
    int reverse(int x) {
        int rev = 0;

        while (x != 0) {
            int lastdigit = x % 10;

            if (rev > INT_MAX / 10 || rev < INT_MIN / 10) {
                return 0;
            }

            rev = (rev * 10) + lastdigit;
            x = x / 10;
        }

        return rev;
    }
};
```

## Complexity Analysis

- **Time Complexity:** O(log |x|)
- **Space Complexity:** O(1)

## Key Learnings

- Extracting digits using modulo
- Reversing an integer
- Handling negative numbers
- Preventing integer overflow

One problem at a time. One day at a time! 🚀
