# Day #10 - Input()
## Problem

In **Python 2**, the expression input() is equivalent to eval(raw _input(prompt)).

Code
```

>>> input()  
1+2
3
>>> company = 'HackerRank'
>>> website = 'www.hackerrank.com'
>>> input()
'The company name: '+company+' and website: '+website
'The company name: HackerRank and website: www.hackerrank.com'

```
***Task***

You are given a polynomial **P** of a single indeterminate (or variable), **x**.<br>
You are also given the values of **x** and **k**. Your task is to verify if **P(x) = k**.

***Constraints***

All coefficients of polynomial **P** are integers.<br>
**x** and **y** are also integers.

***Input Format***

The first line contains the space separated values of **x** and **y**.<br>
The second line contains the polynomial **P**.

***Output Format***

Print True if **P(x) = k**. Otherwise, print False.

***Sample Input***
```

1 4
x**3 + x**2 + x + 1

```
***Sample Output***
```

True

```
***Explanation***

**P(1) = 1<sup>3</sup> + 1<sup>3</sup> + 1 + 1 = 4 = k**<br>
Hence, the output is True.

## Solution
```py
x, k = list(map(int,input().split()))

P = eval(input())

print(P==k)
```
