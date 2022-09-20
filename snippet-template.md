---
title: verify triangle / area
tags: math
expertise: beginner
firstSeen: 2021-06-13T05:00:00-04:00
---

Returns the area of a triangle using heron's equation if the 
triangle is valid

- The function takes in 3 parameters (the sides of a triangle)
- returns the area if all sides are valid and -1 if invalid

```py
def tri_verify(a, b, c):
    import math
    sides = [a, b, c]
    sides.sort()
    if a < 0 or b < 0 or c < 0:
        return -1
    if sides[2] > sides[0] + sides[1]:
        return -1
    else:
        s = (a + b + c) / 2
        area = math.sqrt (s * (s-a) * (s-b) * (s-c))
        return area
# code
```

```py
tri_verify(5,4,8) # 8.18
tri_verify(19,13,12) # 77.07
tri_verify(2,6,11) # -1
tri_verify(10,-11,3) # -1


```

