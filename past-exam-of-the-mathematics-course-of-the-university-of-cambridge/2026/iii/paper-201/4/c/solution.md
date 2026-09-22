<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Let $X_1,X_2,\ldots$ be [independent and identically distributed random variables](../../../../../../independent-and-identically-distributed-random-variables.md) with mean zero and variance one, and let $S_k=\sum_{j=1}^kX_j$. Define the linearly interpolated process

$$
W_n(t)=\frac1{\sqrt n}
\left(S_{\lfloor nt\rfloor}+(nt-\lfloor nt\rfloor)X_{\lfloor nt\rfloor+1}\right),
\qquad0\leq t\leq1.
$$

The [Donsker invariance principle](../../../../../../donsker-s-theorem.md), also called the [functional central limit theorem](../../../../../../donsker-s-theorem.md), states that $W_n$ converges [weakly](../../../../../../convergence-in-distribution.md) in the space $C[0,1]$ with the [uniform norm](../../../../../../supremum-norm.md) to standard [Brownian motion](../../../../../../brownian-motion-split.md).

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
