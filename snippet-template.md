---
title: Binary to Integer
tags: math
expertise: beginner
firstSeen: 2022-09-22T20:41:30+0000
---

Returns the decimal representation of a binary number

- Will return the decimal representation of the binary number 
- passed in. The function will return -1 if an invalid input is given.
- The argument must be wrapped in a string

```py
def binary_to_int(bin_num):
    # code
    try:
        int(bin_num, 2)
    except ValueError:
        return None
    else:
        return int(bin_num, 2)


```

```py
binary_to_int('10001')  # 17
binary_to_int('11110101')  # 245
binary_to_int('232')  # None



```
