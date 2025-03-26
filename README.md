# [LeetCode](https://leetcode.com) practice


## Solved Problems

| | Easy | Medium | Hard | Total |
|:---:|:---:|:---:|:---:|:---:|
| **Accepted** | 1 | 0 | 0 | 1 |
| **Total** | 575 | 1198 | 530 | 2303 |
| **Coverage** | 0.21 % |0 % | 0 % | 0 % |

Python.
1.Two sum
class Solution:
```
    def twoSum(self, nums: List[int], target: int) -> List[int]:
        for i in range(len(nums)):  
            for j in range(i + 1, len(nums)): 
                if nums[i] + nums[j] == target:
                    return [i, j]  
```
9.Palindrome number
class Solution:
```
    def isPalindrome(self, x: int) -> bool:
        return str(x) == str(x)[::-1]
```
