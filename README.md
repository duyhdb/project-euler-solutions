# Project Euler Solutions―projecteuler.net
A collection of my solutions/answers to solve Project Euler problems in Python.

## Anwsers
* [Problem 001](#Problem-001): 233168
* [Problem 002](#Problem-002): 4613732
* Problem 003: 6857
* Problem 004: 906609
* Problem 005: 232792560
* [Problem 006](#Problem-006): 25164150

## Solutions
### Problem 001
```py
sum(x for x in range(1000) if (x % 3 == 0 or x % 5 == 0))  # `generator` better list comp
```
### Problem 002
```py
def fs():
    a, b, c = 0, 1, 0
    while b < 1000000:
        if b % 2 == 0:
          c += b 
        a, b= b, a + b
    print(c)
```
### Problem 006
```py
# The sum of the squares of the first 100 natural numbers
sum(map(lambda i : i * i, range(101)))
```
Or
```py
# Using list comprehension
sum([x for x in range(101)])**2 - sum([x**2 for x in range(101)])
```
