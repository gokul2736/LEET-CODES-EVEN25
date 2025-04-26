# LEET-CODE-WEEKLY SOLUTIONS:
*EASY QUESTIONS ONLY*

## WEEK 1:
```
 a=0
        for b in nums:
            a ^=b
        return a
```

## WEEK 2:
```
a = majority = 0
    for n in nums:
        if majority ==0:
            a=n
        majority += 0 if n == 0 else -1    
    return a
```

## WEEK 3:
```
class Solution(object):
    def isPalindrome(self, s):
        symbols = 'abcdefghijklmnopqrstuvwxyz1234567890'
        a=''
        for b in s.lower():
            if b in symbols:
                a+=b
        return a[::-1] == a        
```

## WEEK 4:
```
class Solution:
    def isPerfectSquare(self, num: int) -> bool:
        return int(num**0.5)==num**0.5
```

## WEEK 5:
```
class Solution(object):
    def isValid(self, s):
        while len(s)>0:
            l = len(s)
            s=s.replace('()','').replace('{}','').replace('[]','')
            if l == len(s): return False
        return True       
```

## WEEK 6:
```

```

## WEEK 7:
```

```

## WEEK 8:
```

```

## WEEK 9:
```

```
