---
{"dg-publish":true,"permalink":"/tutorials/tutorial-1-solutions/"}
---

#### Author: Matthew J. Crossley

#### Last update: 03 March, 2024

``` python
import numpy as np
import matplotlib.pyplot as plt

# 1.
ans_1a = 3.14159
ans_1b = 3
ans_1c = True
ans_1d = 'hello world'
ans_1e = [1, 'a', True]
ans_1f = list(ans_1e)
ans_1f.append(10)
ans_1e = (1, 'a', True)
ans_1h = "can't because tuples are immutable"
ans_1i = {'A': [1, 2, 3], 'B': ('a', 'b', 'c', 'd')}

# NOTE: For the most part these solutions aren't useful
# because you can just copy and run the code yourself to
# check your work. Nevertheless, here they are:

# a: 
# x=7, 
# i=5
# x=5
# for i in [1, 3, 20]:
#   x = i / 2
  
# b 
# len(y) = 8
# y[-1]=6

# c
# x = 10 and y = -10 --> z = 10
# x = -5 and y = 5 --> z = 2
# x = 0 and y = 0 --> z = 2

# d
# 4 times
# i = 3
# x = 6

# e
# x = 10 and y = -10 --> z=2
# x = -5 and y = 5 --> z=3
# x = 0 and y = 0 --> z=1

# f
# inside the function, `x` is 3, `y` is 9, and `z` is
# undefined.
#
# outside the function, `x` and `y` are not defined, and `z`
# is  9.

# g
# outside the functions, `x` and `y` are undefined, and `z`
# is 4
#
# inside `g`, `x` is 4, and `y` is 2
# inside `f`, `x` is 2, and `y` is 4

# h
# f(2, 1, -4) is valid
# f(x=2, 1, -4) throws an error / is invalid
# the wisest way is to name all arguments: f(x=2, y=1, z=-4)
```