---
{"dg-publish":true,"permalink":"/tutorials/tutorial-1/"}
---


#### Last update: 03 March, 2024

## Learning objectives

- Be able to do basic `python` programming.
- Create and use variables of basic data types (`float`, `int`, `str`, `bool`).
- Create and use basic container data types (`list`, `tuple`, `set`, `dict`).
- Create and understand `for` and `while` loops.
- Create and understand conditional flow using `if`, `elif`, `else`.
- Create and understand how to define and use your own custom functions.

## Practice problems

- It’s a good idea to work through these on your own, but if you get very stuck, solutions can be found [here](https://crossley.github.io/cogs3020/tutorials/tutorial_1_solutions.html) [[Tutorials/Tutorial 1 Solutions\|Tutorial 1 Solutions]]

```python
import numpy as np
import matplotlib.pyplot as plt
```

- Create a `float` variable named `ans_1a` that contains the value `3.14159`.
    
- Create an `int` variable named `ans_1b` that contains the value `3`.
    
- Create a `bool` variable named `ans_1c` that contains the value `True`.
    
- Create a `str` variable named `ans_1d` that contains the value `hello world`.
    
- Create a `list` named `ans_1e` that contains the elements `1`, `'a'`, and `True` in that order.
    
- If possible, append the value `10` to the `list` you created in the previous problem and save the result in a variable named `ans_1f`.If not possible, write `ans_1f = 'can't because lists are immutable'`. Be sure not to modify the `ans_1e` variable while doing this.
    
- Create `tuple` named `ans_1g` that contains the elements `1`, `'a'`, and `True` in that order.
    
- If possible, append the value `10` to the `tuple` you created in the previous problem and save the result in a variable named `ans_1h`. If not possible, write `ans_1h = 'can't because tuples are immutable'`. Be sure not to modify the `ans_1g` variable while doing this.
    
- Create a `dict` variable named `ans_1i` with one key named `A` that contains the list `[1, 2, 3]` and another key named `B` that contains the tuple `('a', 'b', 'c', 'd')`.
    

1. Consider the following code chunk:

```python
x = 5
for i in [1, 3, 5]:
  x = i + 2
```

- What is the value of `x` after the loop has finished executing?
- What is the value of `i` after the loop has finished executing?
- Modify the code chunk such that the final value of `x` is 10 and `i` is 20.

2. Consider the following code chunk:

```python
x = 10
y = [1, 2, 3]
while x > 5:
  y.append(x)
  x = x - 1
```

- How many elements does `y` contain after the loop has finished?
- What is the value of the final element in `y` and can you figure this out without executing the code?

3. Consider the following code chunk:

```python
if x > y: 
  z = 10
else:
  z = 2
```

- What is the value of `z` if `x = 10` and `y = -10`
- What is the value of `z` if `x = -5` and `y = 5`
- What is the value of `z` if `x = 0` and `y = 0`

4. Consider the following code chunk:

```python
for i in range(10):
  x = i * 2
  if x > 5:
    break
```

- How many times will this loop run?
- What is the value of `i` and `x` when the loop stops?

5. consider the following code chunk:

```python
if x == y:
  z = 1
elif x > y:
  z = 2
elif x < y:
  z = 3
```

- What is the value of `z` if `x = 10` and `y = -10`
- What is the value of `z` if `x = -5` and `y = 5`
- What is the value of `z` if `x = 0` and `y = 0`

6. Consider the following code chunk:

```python
def f(x):
  y = x**2
  return y

z = f(3)
```

- What are the values of `x`, `y` and `z`?

7. Consider the following code chunk:

```python
def f(x):
  y = x**2
  return y

def g(x):
  y = x - 2
  return y

z = f(g(4))
```

- What are the values of `x`, `y` and `z`?

8. Consider the following code chunk:

```python
def f(x, y, z):
  res = x + y - z
  return res
```

- Is `f(2, 1, -4)` a valid way to call the function `f`?
- Is `f(x=2, 1, -4)` a valid way to call the function `f`?
- What is the wisest way to call the function `f`?