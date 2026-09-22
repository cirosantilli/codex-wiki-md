<h1 id="8/a/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

The finite-partition form of the [law of total expectation](../../../../../../law-of-total-expectation.md) states

$$
\boxed{\mathbb E[X]=\sum_{j:\,\mathbb P(B_j)>0}\mathbb P(B_j)\,\mathbb E[X\mid B_j].}
$$

Because the [events](../../../../../../event.md) form a [partition of a sample space](../../../../../../partition-of-a-sample-space.md) of the [sample space](../../../../../../sample-space.md), $\sum_j\mathbf1_{B_j}=1$ pointwise. Multiply by $X$ and use [linearity of expectation](../../../../../../linearity-of-expectation.md) to obtain

$$
\mathbb E[X]=\sum_j\mathbb E[X\mathbf1_{B_j}]=\sum_{j:\,\mathbb P(B_j)>0}\mathbb P(B_j)\mathbb E[X\mid B_j].
$$

An [event](../../../../../../event.md) of zero [probability](../../../../../../probability.md) contributes zero to the middle expression and is omitted from the final expression, so no undefined [conditional expectation](../../../../../../conditional-expectation.md) is multiplied by zero.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [A](../../a.md)
3. [8](../../../8.md)
4. [Discrete mathematics, continuous mathematics, and probability resit](../../../../discrete-mathematics-continuous-mathematics-and-probability-resit-split.md)
5. [2019](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
