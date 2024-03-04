---
{"dg-publish":true,"permalink":"/tutorials/tutorial-2/"}
---

#### Author: Matthew J. Crossley

#### Last update: 03 March, 2024

## Learning objectives

- Build basic competence with `numpy`

## Practice problems

- It’s a good idea to work through these on your own, but if you get very stuck, solutions can be found [here](https://crossley.github.io/cogs3020/tutorials/tutorial_2_solutions.html) [[Tutorials/Tutorial 2 Solutions\|Tutorial 2 Solutions]]
    
- Create a `numpy.ndarray` with shape `(3,)` and set its elements to `1`, `2`, and `3`, in that order.
    
- Create a `numpy.ndarray` with shape `(3, 1)` and set its elements to `1`, `2`, and `3`, in that order.
    
- Create a `numpy.ndarray` with shape `(3, 2)` and set the elements indexed by `[:, 0]` to `1`, `2`, and `3`, and those indexed by `[:, 1]` to `4`, `5`, `6` in that order.
    
- Create a `numpy.ndarray` with shape `(4, 4)` and set every element to `0` with data type `int`.
    
- Create a `numpy.ndarray` with shape `(4, 4)` and set every element to `1` data type `float`.
    
- Create a `numpy.ndarray` that contains a sequence of `6` evenly spaced numbers starting with the `float` number `1.2` and ending with the `float` number `7.5`.
    
- Create a `numpy.ndarray` that contains the sequence of numbers starting with the `int` number `1` and ending with the `int` number `7` with every `2` increments included.
    
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
```

- For `x` and `y` defined in the following code chunk, compute their element-wise difference.

```python
x = np.array([[1, 2, 3], [4, 5, 6]])
y = np.array([[5, 4, 3], [2, 1, 0]])
```

- Compute the matrix product of `x` and `y.T`.
    
- Use the function `np.max()` to compute the maximum value in the array `x`.
    
- Use the `numpy.ndarray` method `max()` to return the maximum values along the first dimension in the array `y`.
    
- Compute the element-wise square root of the following array `np.array([4, 33, 9])`.
    
- Define `x` and `y` as shown in the following code chunk.
    

```python
x = np.random.randn(3, 4, 2)
y = np.ones(x.shape)
```

- Use slicing or indexing to return the first 2 elements of `x` in dimension `1`, which should result in an array with shape equal to `(2, 4, 2)`.
    
- Use slicing or indexing to return the first element in `x` in dimension `1`, the second element in dimension `2`, and every element in dimension `3`. Your result should be an array with shape equal to `(2, )`.
    
- Concatenate `x` and `y` along the second dimension.
    
- Make a deep copy of `x`, add `10` to every element.
    
- Make a deep copy of `x`, set every element in the first dimension to zero.
    
- Make a deep copy of `x`, use boolean indexing to set every element of `x` that is less than `0.5` to zero.
    
- Create a 2D NumPy array of shape (3, 3) with random integers between 0 and 9.
    
- Create a 1D NumPy array of size 10 with all elements equal to 5.
    
- Create a 2D NumPy array of shape (4, 4) with elements on the main diagonal equal to 1 and all other elements equal to 0.
    
- Create a 1D NumPy array of size 5 with random integers between 0 and 9, then replace all odd numbers with -1.
    
- Create a 2D NumPy array of shape (3, 3) with random floats between 0 and 1, then normalize the array by dividing each element by the sum of all elements.
    
- Create a 1D NumPy array of size 10 with random integers between 0 and 9, then sort the array in descending order.
    
- Create a 2D NumPy array of shape (4, 4) with random integers between 0 and 9, then calculate the mean of each row.
    
- Create a 1D NumPy array of size 5 with random integers between 0 and 9, then calculate the cumulative sum of the array.
    
- Create a 1D NumPy array of size 10 with random integers between 0 and 9, then replace all even numbers with an odd number.
    
- Create a 2D NumPy array of shape (5, 5) with random integers between 0 and 9, then replace the diagonal elements with the average of all elements.
    
- Create a 2D NumPy array of shape (4, 4) with random integers between 0 and 9, then find the location of the maximum value in each row.
    
- Create a 1D NumPy array of size 20 with random integers between 0 and 9, then find the top 5 most frequent values in the array.
    
- Create a 2D NumPy array of shape (3, 3) with random floats between 0 and 1, then find the row with the smallest sum.
    
- Create a 1D NumPy array of size 10 with random integers between 0 and 9, then split the array into 2 smaller arrays such that the first array contains the even numbers and the second array contains the odd numbers.