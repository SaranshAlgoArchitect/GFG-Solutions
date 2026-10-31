## 01. Count Digits in Number

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/count-total-digits-in-a-number/1)

### Problem Description

**Task:** Given a number n, return the count of digits in this number.Examples :Input: n = 1567

#### Examples

##### Example 1

- **Output:**
```text
5
```
- **Explanation:** The number of digits in 99999 is 5.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-10-31 08:19:45
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    int countDigits(int n) {
        // Code here
        if(n==0)  return 1;
        int count=0;
        int w;
        while(n>0){
            w=n%10;
            count++;
            n=n/10;
        }
        return count;
    }
};
```

*Generated on: 31/10/2026, 08:20:24*