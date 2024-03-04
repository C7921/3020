---
{"dg-publish":true,"permalink":"/tutorials/tutorial-2-solutions/"}
---


#### Author: Matthew J. Crossley

#### Last update: 03 March, 2024

```python
import numpy as np
import matplotlib.pyplot as plt
```

- Create a `numpy.ndarray` with shape `(3,)` and set its elements to `1`, `2`, and `3`, in that order.

```python
ans = np.array([1, 2, 3])
```

- Create a `numpy.ndarray` with shape `(3, 1)` and set its elements to `1`, `2`, and `3`, in that order.

```python
ans = np.array([[1, 2, 3]]).T
```

- Create a `numpy.ndarray` with shape `(3, 2)` and set the elements indexed by `[:, 0]` to `1`, `2`, and `3`, and those indexed by `[:, 1]` to `4`, `5`, `6` in that order.

```python
ans = np.array([[1, 2, 3], [4, 5, 6]]).T
```

- Create a `numpy.ndarray` with shape `(4, 4)` and set every element to `0` with data type `int`.

```python
ans = np.zeros((4, 4), dtype=int)
```

- Create a `numpy.ndarray` with shape `(4, 4)` and set every element to `1` data type `float`.

```python
ans = np.ones((4, 4), dtype=float)
```

- Create a `numpy.ndarray` that contains a sequence of `6` evenly spaced numbers starting with the `float` number `1.2` and ending with the `float` number `7.5`.

```python
ans = np.linspace(1.2, 7.5, 6)
```

- Create a `numpy.ndarray` that contains the sequence of numbers starting with the `int` number `1` and ending with the `int` number `7` with every `2` increments included.

```python
ans = np.arange(1, 7, 2)
```

- Follow the instructions in the following code chunk to define `x` and `y`.

```python
tmp = np.array([[1, 2, 3], [4, 5, 6], [7, 8, 9], [10, 11, 12]])
# array([[ 1,  2,  3],
#        [ 4,  5,  6],
#        [ 7,  8,  9],
#        [10, 11, 12]])

# without using np.array(), create a new array that prints
# as follows:
# x = ???
# array([[ 1,  4,  7, 10],
#        [ 2,  5,  8, 11],
#        [ 3,  6,  9, 12]])

# without using np.array(), create a new array that prints
# as follows:
# y = ???
# array([[ 1,  2,  3,  4],
#        [ 5,  6,  7,  8],
#        [ 9, 10, 11, 12]])

x = tmp.T
y = np.reshape(tmp, (3, 4))
```

- For `x` and `y` defined in the following code chunk, compute their element-wise difference.

```python
x = np.array([[1, 2, 3], [4, 5, 6]])
y = np.array([[5, 4, 3], [2, 1, 0]])
ans = x - y
```

- Compute the matrix product of `x` and `y.T`.

```python
ans = np.dot(x, y.T)
```

- Use the function `np.max()` to compute the maximum value in the array `x`.

```python
ans = x.max()
```

- Use the `numpy.ndarray` method `max()` to return the maximum values along the first dimension in the array `y`.

```python
ans = x.max(axis=1)
```

- Compute the element-wise square root of the following array `np.array([4, 33, 9])`.

```python
ans = np.sqrt(np.array([4, 33, 9]))
```

- Define `x` and `y` as shown in the following code chunk.

```python
x = np.random.randn(3, 4, 2)
y = np.ones(x.shape)
```

- Use slicing or indexing to return the first 2 elements of `x` in dimension `1`, which should result in an array with shape equal to `(2, 4, 2)`.

```python
ans= x[:2, :]
```

- Use slicing or indexing to return the first element in `x` in dimension `1`, the second element in dimension `2`, and every element in dimension `3`. Your result should be an array with shape equal to `(2, )`.

```python
ans= x[0, 1, :]
```

- Concatenate `x` and `y` along the second dimension.

```python
ans= np.concatenate((x, y), 1)
```

- Make a deep copy of `x`, add `10` to every element.

```python
ans= np.array(x) + 10
```

- Make a deep copy of `x`, set every element in the first dimension to zero.

```python
ans[0, :, :] = 0
```

- Make a deep copy of `x`, use boolean indexing to set every element of `x` that is less than `0.5` to zero.

```python
ans = np.array(x)
ans[ans < 0.5] = 0
```

- Create a 2D NumPy array of shape (3, 3) with random integers between 0 and 9.

```python
arr = np.random.randint(0, 10, size=(3, 3))
print(arr)
```

```python
## [[0 4 4]
##  [9 0 6]
##  [8 6 7]]
```

- Create a 1D NumPy array of size 10 with all elements equal to 5.

```python
arr = np.ones(10, dtype=int) * 5
print(arr)
```

```python
## [5 5 5 5 5 5 5 5 5 5]
```

- Create a 2D NumPy array of shape (4, 4) with elements on the main diagonal equal to 1 and all other elements equal to 0.

```python
arr = np.eye(4, dtype=int)
print(arr)
```

```python
## [[1 0 0 0]
##  [0 1 0 0]
##  [0 0 1 0]
##  [0 0 0 1]]
```

- Create a 1D NumPy array of size 5 with random integers between 0 and 9, then replace all odd numbers with -1.

```python
arr = np.random.randint(0, 10, size=5)
arr[arr % 2 == 1] = -1
print(arr)
```

```python
## [ 8  8  4  8 -1]
```

- Create a 2D NumPy array of shape (3, 3) with random floats between 0 and 1, then normalize the array by dividing each element by the sum of all elements.

```python
arr = np.random.random((3, 3))
arr_normalized = arr / arr.sum()
print(arr_normalized)
```

```python
## [[0.08469537 0.06644801 0.0822165 ]
##  [0.14145328 0.16949298 0.03448622]
##  [0.15288453 0.13109245 0.13723066]]
```

- Create a 1D NumPy array of size 10 with random integers between 0 and 9, then sort the array in descending order.

```python
arr = np.random.randint(0, 10, size=10)
arr_sorted = np.sort(arr)[::-1]
print(arr_sorted)
```

```python
## [9 9 7 6 5 5 4 3 1 0]
```

- Create a 2D NumPy array of shape (4, 4) with random integers between 0 and 9, then calculate the mean of each row.

```python
arr = np.random.randint(0, 10, size=(4, 4))
arr_row_mean = np.mean(arr, axis=1)
print(arr_row_mean)
```

```python
## [6.5  3.75 5.5  3.5 ]
```

- Create a 1D NumPy array of size 5 with random integers between 0 and 9, then calculate the cumulative sum of the array.

```python
arr = np.random.randint(0, 10, size=5)
arr_cumsum = np.cumsum(arr)
print(arr_cumsum)
```

```python
## [ 4  4 10 10 16]
```

- Create a 1D NumPy array of size 10 with random integers between 0 and 9, then replace all even numbers with an odd number.

```python
arr = np.random.randint(0, 10, size=10)
mask = arr % 2 == 0
arr[mask] += 1
print(arr)
```

```python
## [1 1 9 5 3 7 9 7 9 7]
```

- Create a 2D NumPy array of shape (5, 5) with random integers between 0 and 9, then replace the diagonal elements with the average of all elements.

```python
arr = np.random.randint(0, 10, size=(5, 5))
mask = np.eye(5, dtype=bool)
arr[mask] = arr.mean()
print(arr)
```

```python
## [[4 5 0 8 2]
##  [1 4 9 0 7]
##  [8 6 4 7 4]
##  [4 4 4 4 3]
##  [1 1 9 3 4]]
```

- Create a 2D NumPy array of shape (4, 4) with random integers between 0 and 9, then find the location of the maximum value in each row.

```python
arr = np.random.randint(0, 10, size=(4, 4))
max_indices = np.argmax(arr, axis=1)
print(max_indices)
```

```python
## [1 2 3 0]
```

- Create a 1D NumPy array of size 20 with random integers between 0 and 9, then find the top 5 most frequent values in the array.

```python
arr = np.random.randint(0, 10, size=20)
unique, counts = np.unique(arr, return_counts=True)
top_indices = np.argsort(counts)[-5:]
top_values = unique[top_indices][::-1]
print(top_values)
```

```python
## [7 6 5 4 9]
```

- Create a 2D NumPy array of shape (3, 3) with random floats between 0 and 1, then find the row with the smallest sum.

```python
arr = np.random.random((3, 3))
row_sums = np.sum(arr, axis=1)
min_index = np.argmin(row_sums)
print(arr[min_index])
```

```python
## [0.24993658 0.4590776  0.27533847]
```

- Create a 1D NumPy array of size 10 with random integers between 0 and 9, then split the array into 2 smaller arrays such that the first array contains the even numbers and the second array contains the odd numbers.

```python
arr = np.random.randint(0, 10, size=10)
even = arr[arr % 2 == 0]
odd = arr[arr % 2 == 1]
print(even, odd)
```

```python
## [4 0 0 4 2] [7 3 5 7 3]
```