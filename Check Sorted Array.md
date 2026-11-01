## 01. Check Sorted Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/check-if-an-array-is-sorted0701/1)

### Problem Description

**Task:** Given an array arr[], check whether it is sorted in non-decreasing order. Return true if it is sorted otherwise false.Examples:Input: arr[] = [10, 20, 30, 40, 50]

#### Examples

##### Example 1

- **Output:**
```text
false
```
- **Explanation:** The given array is not sorted.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (1)

#### Solution 1 (C++)

- **Submitted:** 2026-11-01 15:10:40
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    bool isSorted(vector<int>& arr) {
        // code here
        int n=arr.size();
        for(int i=1;i<n;i++){
            if(arr[i]>=arr[i-1]){
                
            }
            else {
                return false;
            }
        }
        return true;
    }
};
```

*Generated on: 01/11/2026, 15:12:30*