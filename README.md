# Task-10 NumPy-Indexing-and-Slicing.

## Overview
This project demonstrates how to access elements, rows, columns, and ranges in NumPy arrays using indexing and slicing.

## Objectives
- Practice positive and negative indexing in one-dimensional arrays.
- Access individual elements and rows in two-dimensional arrays.
- Perform at least five slicing operations.
- Understand how start, stop, and step work in slicing.

## Tools Used
- Python
- NumPy
- Jupyter Notebook / Google Colab

## Installation
If NumPy is not installed, run:

```python
!pip install numpy
```

## Examples

### 1. One-dimensional indexing

```python
import numpy as np

arr = np.array([10, 20, 30, 40, 50])

print("Array:", arr)
print("First element:", arr[0])
print("Third element:", arr[2])
print("Last element:", arr[-1])
print("Second-last element:", arr[-2])
```

### 2. Two-dimensional indexing

```python
arr2 = np.array([
    [10, 20, 30],
    [40, 50, 60],
    [70, 80, 90]
])

print("First row:", arr2[0])
print("Second row:", arr2[1])
print("Element at row 1, column 2:", arr2[1, 2])
print("Last element:", arr2[-1, -1])
```

### 3. Five slicing examples

```python
arr = np.array([10, 20, 30, 40, 50])

# Example 1: Select elements from index 1 to index 3
print(arr[1:4])     # [20 30 40]

# Example 2: Select the first three elements
print(arr[:3])      # [10 20 30]

# Example 3: Select elements from index 2 to the end
print(arr[2:])      # [30 40 50]

# Example 4: Select every second element
print(arr[::2])     # [10 30 50]

# Example 5: Reverse the array
print(arr[::-1])    # [50 40 30 20 10]
```

### 4. Two-dimensional slicing

```python
arr2 = np.array([
    [10, 20, 30],
    [40, 50, 60],
    [70, 80, 90]
])

print("First two rows:")
print(arr2[:2, :])

print("First two columns:")
print(arr2[:, :2])

print("First two rows and first two columns:")
print(arr2[:2, :2])
```

### 5. Optional real dataset: Iris

If scikit-learn is available, use the Iris dataset to practice indexing on real numerical data:

```python
from sklearn.datasets import load_iris

iris = load_iris()
data = iris.data

print("First five rows:")
print(data[:5])

print("First column:")
print(data[:, 0])

print("First five rows, first two columns:")
print(data[:5, :2])
```

Install scikit-learn if needed:

```python
!pip install scikit-learn
```

## Key Concepts
- Python indexing starts at `0`.
- Negative indices count backward from the end; `-1` selects the last element.
- In `arr[start:stop:step]`, the `stop` index is excluded.
- For 2D arrays, use `arr[row, column]`.
- In 2D slicing, `:` selects all elements along that dimension.

## How to Run
1. Open Jupyter Notebook or Google Colab.
2. Create a notebook named `NumPy_Indexing_and_Slicing.ipynb`.
3. Run the examples in order.
4. Confirm the outputs match the comments.
5. Save the notebook and add it to your GitHub repository.

## Repository Name
`numpy-indexing-and-slicing`

## Author
Add your name here.
