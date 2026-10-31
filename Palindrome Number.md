## 01. Palindrome Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/palindrome0746/1)

### Problem Description

**Task:** You are given an integer n. Your task is to find if it is a palindrome. Examples:Input: n = 555

#### Examples

##### Example 1

- **Output:**
```text
trueExplanation: if number is palindrome, mainly ignore sign.
```

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(d), d is number of digits in nAuxiliary Space: O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-10-31 08:42:21
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    bool isPalindrome(int n) {
        int digit;
        int reverse=0;
        int original=n;
        while(n!=0){
            digit=n%10;
            reverse=reverse*10+digit;
            n=n/10;
        }
        if(original==reverse){
            return true;
        }
        else{
            return false;
        }
    }
};
```

*Generated on: 31/10/2026, 08:45:49*