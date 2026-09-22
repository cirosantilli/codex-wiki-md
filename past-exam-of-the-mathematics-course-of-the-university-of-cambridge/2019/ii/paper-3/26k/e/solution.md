<h1 id="26k/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

The displayed density is that of a [gamma distribution](../../../../../../gamma-distribution.md) with shape $k+1$ and rate one. Put

$$
K=\sum_{i=1}^nk_i.
$$

By the [additivity of independent gamma distributions with a common rate](../../../../../../additivity-of-independent-gamma-distributions-with-a-common-rate.md),

$$
X_1+\cdots+X_n\sim\operatorname{Gamma}(K+n,1).
$$

Equivalently, the [independence of random variables](../../../../../../independent-random-variables.md) makes the [Laplace transform of a nonnegative random variable](../../../../../../laplace-transform-of-a-nonnegative-random-variable.md) of the sum equal

$$
\prod_{i=1}^n(1+s)^{-(k_i+1)}
=(1+s)^{-(K+n)}.
$$

Therefore the required [probability density function](../../../../../../probability-density-function.md) is

$$
\boxed{
f_{X_1+\cdots+X_n}(x)
=\mathbf1_{\{x>0\}}
\frac{x^{K+n-1}e^{-x}}{(K+n-1)!}.}
$$

## ↑ Ancestors (11)

1. [E](../e.md)
2. [26K](../../26k.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
