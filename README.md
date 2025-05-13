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
class Solution:
    def findKthPositive(self, arr, k):
        for a in arr:
            if a <= k: k += 1
        return k
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

## WEEK 9:  Plus One
```
class Solution(object):
    def plusOne(self, d):
        for i in range(len(d)-1, -1, -1):
            if d[i] < 9:
                d[i] += 1; return d
            d[i] = 0
        return [1]+d

```

## WEEK 10:  Valid Anagram
```
class Solution:
    def isAnagram(self, s, t):
        return sorted(s) == sorted(t)
```

## WEEK 11:  Length of Last Word
```
class Solution:
    def lengthOfLastWord(self, s):
        return len(s.strip().split()[-1])
```

## WEEK 12:
```
class Solution:
    def searchInsert(self, nums: List[int], target: int) -> int:
        for i in range(len(nums)):
            if target<=nums[i]:
                return i
            else:
                continue
        return i+1
```

## WEEK 13:
```

```
