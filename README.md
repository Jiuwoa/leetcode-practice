# [LeetCode](https://leetcode.com) practice


## Solved Problems

| | Easy | Medium | Hard | Total |
|:---:|:---:|:---:|:---:|:---:|
| **Accepted** | 1 | 0 | 0 | 1 |
| **Total** | 575 | 1198 | 530 | 2303 |
| **Coverage** | 0.21 % |0 % | 0 % | 0 % |

#Python

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

#Golang

1.Two sum
class Solution:
```
func twoSum(nums []int, target int) []int {
    numMap := make(map[int]int) 

	for i, num := range nums {
		complement := target - num 
		if index, found := numMap[complement]; found { 
			return []int{index, i} 
		}
		numMap[num] = i
	}
	return nil

}
```

#Rust

1.Two sum
class soiution
```
use std::collections::HashMap;

impl Solution {
    pub fn two_sum(nums: Vec<i32>, target: i32) -> Vec<i32> {
        let mut map = HashMap::new();

        for (i, num) in nums.iter().enumerate() {
            let complement = target - num;

            if let Some(&index) = map.get(&complement) {
                return vec![index as i32, i as i32];
            }

            map.insert(num, i);
        }

        vec![]
    }
}
```

