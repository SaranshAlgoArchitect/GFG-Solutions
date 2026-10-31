## 01. Armstrong Numbers

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/armstrong-numbers2727/1)

### Problem Description

**Task:** You are given a 3-digit number n, Find whether it is an Armstrong number or not.An Armstrong number of three digits is a number such that the sum of the cubes of its digits is equal to the number itself. 371 is an Armstrong number since 3³ + 7³ + 1³ = 371. Examples:Input: n = 153

#### Examples

##### Example 1

- **Output:**
```text
true
```
- **Explanation:** 153 is an Armstrong number since 1³ + 5³ + 3³ = 153.

##### Example 2

- **Input:**
```text
n = 372
```
- **Output:**
```text
false
```
- **Explanation:** 100 is not an Armstrong number since 1³ + 0³ + 0³ = 1.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(1)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-10-31 09:13:09
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    bool armstrongNumber(int n) {
        // code here
        int count=0;
        int original=n;
        int temp=n;
        while(temp>0){
            count++;
            temp/=10;
        }
        
        int digit;
        int sum=0;
        while(n>0){
            digit=n%10;
            sum=sum+(pow(digit,count));
            n=n/10;
        }
        
        if(original==sum){
            return true;
        }
        else{
            return false;
        }
    }
};
```

*Generated on: 31/10/2026, 09:13:40*