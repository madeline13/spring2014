---
layout: post
author: madeline13
title: Madeline's Codingbat Post
---

## My Codingbat 2

![] http://i.imgur.com/l3sQqbS.png

This wasn't me at my most brilliant, but I did my best.

## lucky_sum

Given 3 int values, a b c, return their sum. However, if one of the values is 13 then it does not count towards the sum and values to its right do not count. So for example, if b is 13, then both b and c do not count.

For this, I simply went through all scenarios, which was possible because the problem gave only 3 values.

```
def lucky_sum(a, b, c):
  if a == 13:
    return 0
  if b == 13:
    return a
  if c == 13:
    return a + b
  else:
    return a + b + c
```

## lone_sum

Given 3 int values, a b c, return their sum. However, if one of the values is the same as another of the values, it does not count towards the sum.

Just like in the problem above, this had three values, so I simply had to go through the scenarios.  Probably, though, a loop would have done it better.

```
def lone_sum(a, b, c):
 if a == b == c:
   return 0
 if a == b:
   return c
 if a == c:
   return b
 if b == c:
   return a
 else:
   return a + b + c
```

## cat_dog

Return True if the string "cat" and "dog" appear the same number of times in the given string.

I found the answer to this one online.  str.count is a built-in function for Python.  The reason there are not so many others is the fact that it would take infinite functions to encompass everything that can be done with Python.

```
def cat_dog(str):
  if str.count("dog") == str.count("cat"):
    return True
  else:
    return False
```
    
