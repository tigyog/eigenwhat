---
type: course
id: C-a63ebf065d
slug: eigenwhat
priceUsdDollars: 5
---

# Eigenwhat?

## Linear algebra for machine learning

You want to build AIs,
but got stuck with matrix multiplication?
Maybe you picked up a linear algebra textbook, but got stuck on "determinants"?
This course is for you!
I'll skip over the stuff you don't need (like eigenwotsits),
and I'll add the things the textbooks don't cover, like "tensors" and "broadcasting".
By the end, you'll be able to
follow ML tutorials like [GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY),
and use the essentials of `numpy` comfortably.

The only prerequisite is that you’re comfortable coding with numbers and arrays.
I emphasize Python code like `[1,2]` instead of math squiggles like $[\begin{smallmatrix}1\\2\end{smallmatrix}]$.
I emphasize intuition over proof.
I motivate each concept with machine-learning examples.

::buy[Eigenvalue: $5]

## What's in the course?

:::chapterlink{path="./vectors.md"}
# Vectors

In this chapter, we'll see the equivalence of three things:
arrays of numbers, points in space, and arrows.
Vectors are all of these!
We'll use "word embeddings" as an example, and see what "addition" and "multiplication" mean for vectors.
You'll re-invent "scalar multiplication" in Python, motivated by "rescaling" our word embeddings.
:::

:::chapterlink
# The dot product

How "similar" are two vectors?
If we see the vectors as arrows, we can say they're similar if they point in the same direction.
You'll re-invent the "dot product", which can tell us the angle between two vectors.
You'll implement it in Python and use it to compare word similarities.
:::

:::chapterlink{path="./matrices.md"}
# Matrices

In this chapter, we'll see how to transform vectors:
squashing, flipping, and rotating.
You'll re-invent the concept of a "matrix",
and implement "matrix-vector multiplication" in Python.
:::

:::chapterlink
# Matrix multiplication

In this chapter, we'll apply multiple transformations in sequence.
You'll re-invent "matrix-matrix multiplication" yourself,
then implement it in Python.
:::

:::chapterlink
# Tensors

A tensor is just a spreadsheet on steroids!
We'll see a big tensor with shape `(batch, time, heads, channels)`.
You'll re-invent "reshaping" tensors in Python.
:::

:::chapterlink
# Broadcasting

Earlier we learned that we could multiply a vector by a number:
rather than giving us an error, it scales the vector!
In this chapter, you'll re-invent something called "broadcasting",
which generalizes this idea.
You won't see this notation in textbooks, but it's an essential part of machine learning code.
:::

Here's the essential `numpy` API that you'll be familiar with after completing this course:

```python
import numpy as np

# Vectors
vector_1 = np.array([1, 2, 3])
vector_2 = np.array([4, 5, 6])

# Vector addition
vector_sum = vector_1 + vector_2

# Scalar multiplication
scaled_vector = 2 * vector_1

# Dot product
dot_product = np.dot(vector_1, vector_2)

# Matrices
matrix = np.array([[1, 2], [3, 4]])

# Matrix-vector multiplication
transformed_vector = np.dot(matrix, vector_1)

# Matrix-matrix multiplication
matrix_1 = np.array([[1, 2], [3, 4]])
matrix_2 = np.array([[5, 6], [7, 8]])
matrix_product = np.dot(matrix_1, matrix_2)

# Tensors
tensor = np.random.rand(2, 3, 4, 5)

# Reshaping tensors
reshaped_tensor = tensor.reshape((2, 12, 5))

# Transpose
transposed_tensor = tensor.transpose((0, 2, 1, 3))

# Broadcasting
broadcasted_sum = vector_1 + 2
```
