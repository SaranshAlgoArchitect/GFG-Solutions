## 01. Second Largest

The problem can be found at the following link: [Question Link](https://www.geeksforgeeks.org/problems/second-largest3735/1)

### Problem Description

**Task:** Given an array of positive integers arr[], return the second largest element from the array. If the second largest element doesn't exist then return -1.Note: The second largest element should not be equal to the largest element.Examples:Input: arr[] = [12, 35, 1, 10, 34, 1]

#### Examples

##### Example 1

- **Output:**
```text
-1
```
- **Explanation:** The largest element of the array is 10 and the second largest element does not exist.

### Time and Auxiliary Space Complexity

- **Expected Time Complexity:** O(n)
- **Expected Auxiliary Space Complexity:** O(1)

### Accepted Solutions (2)

#### Solution 1 (C++)

- **Submitted:** 2026-11-01 14:52:33
- **Status:** Correct
- **Marks:** 0

```cpp
class Solution {
  public:
    int getSecondLargest(vector<int> &arr) {
        // code here
        int largest=arr[0];
        int s_largest=-1;
        int n=arr.size();
        for(int i=0;i<n;i++){
            if(arr[i]>largest){
                s_largest=largest;
                largest=arr[i];
            }
            else if(arr[i]<largest && arr[i]>s_largest){
                s_largest=arr[i];
            }
        }
        return s_largest;
    }
};
```

#### Solution 2 (C++)

- **Submitted:** 2026-10-01 06:38:52
- **Status:** Correct
- **Marks:** 2

```cpp
class Solution {
  public:
    int getSecondLargest(vector<int> &arr) {
        // code here
        //largest element
        int ans=-1;
        int n=arr.size();
        for(int i=0;i<n;i++){
            if(arr[i]>ans){
                ans=arr[i];
            }
        }
        
        //second largest
        int second =-1;
        for(int j=0;j<n;j++){
            if(arr[j]!=ans){
                
                second=max(second,arr[j]);
            }
        }
        return second;
    }
};
```

*Generated on: 01/11/2026, 14:53:02*