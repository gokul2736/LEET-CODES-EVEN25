# LEET-CODE-SOLS:
*EASY QUESTIONS*

### 1st  two lines (Predefined Function) avasaram ledu chadivi waste eh... 

## WEEK 1:  SINGLE NUMBER 
```
class Solution(object):
    def singleNumber(self, nums):
        a=0
        for b in nums:
            a ^=b
        return a    
       
       
nums_input = input()
nums = list(map(int, nums_input.split()))
sol = Solution()
result = sol.singleNumber(nums)
print(result)
```

## WEEK 2:  Majority Element
```
a = majority = 0
    for n in nums:
        if majority ==0:
            a=n
        majority += 0 if n == 0 else -1    
    return a
```

## <p align="center"><strong>OR</strong></p>

```
from collections import Counter
from typing import List

def majorityElement(nums: List[int]) -> int:
    count=Counter(nums)
    for i in count:
        if count[i] > len(nums)/2:
            return(i)
```

## WEEK 3:  Valid Palindrome
```
class Solution(object):
    def isPalindrome(self, s):
        st=""
        for i in s:
            if i.isalnum():
                st+=i.lower()
        return st==st[::-1]              
```

## WEEK 4:  Perfect square
```
class Solution:
    def isPerfectSquare(self, num: int) -> bool:
        return int(num**0.5)==num**0.5
```

## WEEK 5:  Valid Parentheses
```
class Solution(object):
    def isValid(self, s):
        while len(s)>0:
            l = len(s)
            s=s.replace('()','').replace('{}','').replace('[]','')
            if l == len(s): return False
        return True           
```

## WEEK 6:  Kth Missing Positive Number
```
from typing import List
class Solution:
    def findKthPositive(self, arr: List[int], k: int) -> int:
        for i,x in enumerate(arr):
            if x > i+k:
                return i+k
        return len(arr) + k
```

## WEEK 7:  Squares of a Sorted Array
```
class Solution(object):
    def sortedSquares(self,nums):
        ans=(num*num for num in nums)
        ans=sorted(ans)
        return ans
```

## WEEK 8:  Climbing Stairs
```
class Solution:
    def climbStairs(self, n: int) -> int:
        if n==0 or n==1:
            return 1
        return self.climbStairs(n-1) + self.climbStairs(n-2)
```

## WEEK 9:
```

```

## WEEK 10:
```

```

## WEEK 11:
```

```

## WEEK 12:
```

```
