## 01. Largest in Array

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/largest-element-in-array4009/1)

### Problem Description

**Task:** Given an array arr[]. The task is to find the largest element and return it.Examples:Input: arr[] = [1, 8, 7, 56, 90]

#### Examples

##### Example 1

- **Output:**
```text
10
```
- **Explanation:** There is only one element which is the largest.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (3)

#### Solution 1 (C++)

- **Submitted:** 2026-11-01 14:33:51
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    int largest(vector<int> &arr) {
        // code here
        int n=arr.size();
        int largest =arr[0];
        for(int i=1;i<n;i++){
            if(arr[i]>largest){
                largest=arr[i];
            }
        }
        return largest;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-11-01 14:31:55
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    int largest(vector<int> &arr) {
        // code here
        int n=arr.size();
        int largest =arr[0];
        for(int i=1;i<n;i++){
            if(arr[i]>largest){
                largest=arr[i];
            }
        }
        return largest;
    }
};
```

#### Solution 3 (C++)

- **Submitted:** 2026-09-19 09:08:21
- **Status:** Correct
- **Marks:** 1

```cpp
class Solution {
  public:
    int largest(vector<int> &arr) {
        // code here
        int i;
        int max = arr[0];
        int n = arr.size();
        for(i=1;i<n;i++){
            if(arr[i]>max){
                max=arr[i];
            }
        }
        return max;
    }
};
```

*Generated on: 01/11/2026, 14:34:19*