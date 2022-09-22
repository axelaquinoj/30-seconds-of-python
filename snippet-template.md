---
title: Quadratic formula
tags: math
expertise: beginner
firstSeen: 2022-09-22T20:41:30+0000
---

returns the result of the quadratic formula

- Given the arguments (a,b,c) these values will be used
- to calculate the result of the quadratic equation.
- Returns none if the formulas return an imaginary number

```py
def quadratic(a, b, c):
    import math
    try:
        formula1 = ((-b + (math.sqrt(b ** 2 - (4 * a * c)))) / (a * 2))
        formula2 = ((-b - (math.sqrt(b ** 2 - (4 * a * c)))) / (a * 2))
    except ValueError:
        return None
    return formula1, formula2
```

```py
quadratic(4,6,7)  # None
quadratic(6,9,3)  # (-0.5,-1.0)
quadratic(23,43,11)  # (-0.3058488634135029, -1.5637163539778014)
quadratic(16,76,-14)  # (0.1775722320827673, -4.927572232082767)
```
