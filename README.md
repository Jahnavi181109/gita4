# *PATHI JAHNAVI*
# *2023UCP1595*
# *GIT ASSIGNMENT-4*

---

# Vector Dot-Product Implementation

This repository demonstrates the implementation of the vector dot-product algorithm. It includes mathematical expressions, an example code snippet, and a comparison of algorithm versions.



## Table of Contents
- [Introduction](#introduction)
- [Mathematical Expression](#mathematical-expression)
- [Code Snippet](#code-snippet)
- [Diagram](#diagram)
- [Comparison Table](#comparison-table)



## Introduction

The **vector dot-product**[^1] is a mathematical operation that takes two equal-length sequences of numbers (usually coordinate vectors) and returns a single number. It is widely used in applications such as graphics, physics, and machine learning.



## Mathematical Expression

The dot product of two vectors **A** and **B** is defined as:

$$
\text{Dot Product} = \sum_{i=1}^{n} A_i \times B_i
$$

Where:

- $A = [a_1, a_2, \dots, a_n]$
- $B = [b_1, b_2, \dots, b_n]$

> [!NOTE]
> We can multiply only two vectors at a time.


## Code Example(Python)
1. Without numpy[^2] ->

```
def dot_product(vector_a, vector_b):
    return sum(a * b for a, b in zip(vector_a, vector_b))

vector_a = [1, 2, 3]
vector_b = [4, 5, 6]
result = dot_product(vector_a, vector_b)
print("Dot Product:", result)
```

2. With numpy ->

```
import numpy as np
 
a = 3 + 1j
b = 7 + 6j
 
print(np.dot(a, b))
```

## Diagram

> Below is a diagram illustrating the process of calculating the dot product:

![](https://www.geeksforgeeks.org/wp-content/ql-cache/quicklatex.com-09b8cd354f24a03b37937193ada781b5_l3.svg)

![](https://www.geeksforgeeks.org/wp-content/ql-cache/quicklatex.com-744b63e8b12f771a424e7b392e7823ec_l3.svg)

![](https://www.geeksforgeeks.org/wp-content/ql-cache/quicklatex.com-f17cd27814e5e0debb8fc6dc5a034212_l3.svg)

> Example

![](https://www.geeksforgeeks.org/wp-content/ql-cache/quicklatex.com-a98a9faf3d30c6ccf595025c7835288f_l3.svg)

## Comparison Table

| using numpy | wihtout numpy |
| ----------- | ------------- |
| The sum of the products of related items in two vectors or matrices is computed using the mathematical operation known as the dot product in Python. Both using and without the numpy module, Python may implement the dot product.| Without Numpy we build two Python lists, a and b, and then use a for loop and the sum() method to compute their dot product.|

| Algorithm Version       | Time Complexity | Space Complexity | Notes                       |
|--------------------------|-----------------|------------------|-----------------------------|
| Basic Implementation     | \(O(n)\)      | \(O(1)\)       | Iterative approach.         |
| Optimized Implementation | \(O(n)\)      | \(O(1)\)       | Uses NumPy for performance. |


> [!TIP]
> Use numpy for better results.

---

- [x] Introduction
- [x] Mathematical Expression
- [x] Code Snippet
- [x] Diagram
- [x] Comparison Table

[^1]: We also have cross product
[^2]: numpy is a package available in python
