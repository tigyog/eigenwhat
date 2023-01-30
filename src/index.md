---
type: course
id: C-a63ebf065d
slug: eigenwhat
---

# Eigenwhat?

## Linear algebra for machine learning

You want to build AIs,
but got stuck with matrix multiplication?
Maybe you picked up a linear algebra textbook, but got stuck on "determinants"?
This course is for you!
I'll skip over the stuff you don't need (like eigenwotsits),
and I'll add the things the textbooks don't cover, like tensors and broadcasting.
By the end, you'll be able to follow ML tutorials like [GPT from scratch](https://www.youtube.com/watch?v=kCc8FmEb1nY).

The only prerequisite is that you’re comfortable coding with numbers and arrays.
I emphasize Python code like `[1,2]` instead of math squiggles like $[\begin{smallmatrix}1\\2\end{smallmatrix}]$.
I emphasize intuition over proof.
I motivate each concept with machine-learning examples.

:::chapterlink{path=./vectors.md}
# Vectors

In this chapter, we'll see the equivalence of three things:
arrays of numbers, points in space, and arrows.
You'll implement "scalar multiplication" in Python.
:::

:::chapterlink
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

A tensor is just a spreadsheet on steroids.
You'll re-implement "reshaping" them in Python.
:::

:::chapterlink
# Broadcasting

Earlier we learned that we could multiply a vector by a number:
rather than giving us an error, it scales the vector!
Modern libraries like `numpy` generalize this with a trick called "broadcasting".
You won't see this notation in textbooks, but it's an essential part of machine learning code.
:::