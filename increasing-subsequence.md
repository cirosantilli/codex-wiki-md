# Increasing subsequence

↑ **Parent:** [Combinatorics](combinatorics-split.md)

An [increasing subsequence](increasing-subsequence.md) of a finite [sequence](sequence.md) $x=(x_1,\ldots,x_n)$ in a [totally ordered set](totally-ordered-set.md) selects indices $1\leq i_1<\cdots<i_m\leq n$ such that

$$
x_{i_1}\leq x_{i_2}\leq\cdots\leq x_{i_m}.
$$

Here “increasing” means weakly increasing, also called nondecreasing: equal values are allowed, but indices must increase strictly. This is the convention of [Liben-Nowell, Vee and Zhu, Finding Longest Increasing and Common Subsequences in Streaming Data, section 1](https://cs.carleton.edu/faculty/dlibenno/papers/lis-lcs/lislcs.pdf). A [strictly increasing subsequence](strictly-increasing-subsequence.md) instead requires $x_{i_1}<\cdots<x_{i_m}$. Always check which convention an [algorithm](algorithm-split.md) uses, especially when values repeat.

An [increasing subsequence](increasing-subsequence.md) may skip positions; it neither rearranges values nor requires consecutive positions. Consider the deliberately constructed example

$$
x=(4,1,3,2,2,5,0).
$$

The indices $(2,4,5,6)$ select $(1,2,2,5)$, an [increasing subsequence](increasing-subsequence.md) of length four. The indices $(2,3,6)$ select $(1,3,5)$, a [strictly increasing subsequence](strictly-increasing-subsequence.md) of length three. In contrast, $(0,1,2,2,3,4,5)$ rearranges the input and is not a [subsequence](subsequence.md). The longest consecutive nondecreasing block is $(2,2,5)$, of length three; requiring consecutive positions would therefore solve a different problem.

Think of an [increasing subsequence](increasing-subsequence.md) as preserving ordered observations while skipping interruptions. For the example, discarding $4,3,0$ leaves four observations with no downward step. The [longest increasing subsequence](longest-increasing-subsequence.md) asks how much of the original order can be kept. This is an order comparison, rather than a claim about the size of upward or downward changes: replacing all values by their squares when the values are nonnegative leaves every allowed selection unchanged. More generally, any strictly order-preserving relabeling has this property.

**Table of contents**

- [Longest increasing subsequence](longest-increasing-subsequence.md)
  - [Minimum-tail table for increasing subsequences](minimum-tail-table-for-increasing-subsequences.md)
- [Strictly increasing subsequence](strictly-increasing-subsequence.md)

## ↑ Ancestors (4)

1. [Combinatorics](combinatorics-split.md)
2. [Area of mathematics](area-of-mathematics.md)
3. [Mathematics](mathematics-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Increasing subsequence](increasing-subsequence.md)
- [Longest increasing subsequence](longest-increasing-subsequence.md)
