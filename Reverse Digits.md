## 01. Reverse Digits

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/reverse-digit0316/1)

### Problem Description

**Task:** You are given an integer n. Your task is to reverse the digits, ensuring that the reversed number has no leading zeroes.

#### Examples

##### Example 1

- **Input:**
```text
n = 122
```
- **Output:**
```text
221
```
- **Explanation:** By reversing the digits of number, number will change into 221.

##### Example 2

- **Input:**
```text
n = 200
```
- **Output:**
```text
2
```
- **Explanation:** By reversing the digits of number, number will change into 2.

##### Example 3

- **Input:**
```text
n = 12345
```
- **Output:**
```text
54321
```
- **Explanation:** By reversing the digits of number, number will change into 54321.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(log n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-10-31 08:33:37
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int reverseDigits(int n) {
        // Code here
        int reverse=0;
        int digit;
        while(n!=0){
            digit=n%10;
            reverse=reverse*10+digit;
            n=n/10;
        }
        return reverse;
    }
};
```

*Generated on: 31/10/2026, 08:36:45*