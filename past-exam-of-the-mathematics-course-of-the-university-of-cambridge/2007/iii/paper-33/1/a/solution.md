<h1 id="1/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [filtered probability space](../../../../../../filtered-probability-space.md) $([0,1),\mathcal B([0,1)),(\mathcal F_n),\lambda)$, with its half-open [dyadic intervals](../../../../../../dyadic-interval.md). Complete the initial definition by putting $X_0=\mu([0,1))$. This is the same cell-average formula at level zero, where the only cell is $[0,1)$.

The function $X_n$ is $\mathcal F_n$-measurable and nonnegative. Its [expectation](../../../../../../expected-value.md) is

$$
\mathbb E_\lambda X_n=\sum_{k=0}^{2^n-1}2^n\mu(D_k^n)\lambda(D_k^n)=\mu([0,1))<\infty.
$$

Every parent cell is the disjoint union of its two half-open child cells. On $D_k^n$, the [conditional expectation](../../../../../../conditional-expectation.md) of $X_{n+1}$ is its cell average:

$$
\frac{1}{\lambda(D_k^n)}\int_{D_k^n}X_{n+1}\,d\lambda
=2^n\left[\mu(D_{2k}^{n+1})+\mu(D_{2k+1}^{n+1})\right]
=2^n\mu(D_k^n).
$$

Thus **$\mathbb E[X_{n+1}\mid\mathcal F_n]=X_n$**, including at $n=0$. This proves that $X$ is a [nonnegative martingale](../../../../../../nonnegative-martingale.md), specifically the [dyadic density martingale](../../../../../../dyadic-density-martingale.md). The half-open endpoints are essential to the disjoint partition for an arbitrary [measure](../../../../../../measure.md), which may have atoms.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [1](../../1.md)
3. [Paper 33](../../../paper-33-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
