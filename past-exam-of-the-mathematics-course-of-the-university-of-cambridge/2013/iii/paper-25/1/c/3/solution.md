<h1 id="1/c/3/solution">Solution</h1>

↑ **Parent:** [3](../3.md)

Let $\Delta_j=W_{t_j}-W_{t_{j-1}}$ for $1\le j\le n$. These increments are jointly normal, because each is obtained by evaluating the [isonormal Gaussian process](../../../../../../../isonormal-gaussian-process.md) on an interval indicator. Indicators of distinct intervals are orthogonal in $L^2([0,\infty))$, so

$$
\operatorname{Cov}(\Delta_j,\Delta_k)=0\qquad(j\ne k).
$$

By [uncorrelated jointly Gaussian variables are independent](../../../../../../../uncorrelated-jointly-normal-variables-are-independent.md), **the increments on all these disjoint intervals are independent**. Reversing the sign of the first increment, as in the printed list, preserves this independence.

The three requested properties have now been obtained without an existence theorem for [Brownian motion](../../../../../../../brownian-motion-split.md). One can also obtain continuous paths: the [Gaussian fourth moment](../../../../../../../gaussian-fourth-moment.md) gives $\mathbb E|W_t-W_s|^4=3|t-s|^2$. The [Kolmogorov continuity theorem](../../../../../../../kolmogorov-continuity-theorem.md) therefore supplies a continuous modification on every finite time interval, which can be chosen consistently on the half-line. Modification preserves every finite-dimensional distribution and hence the independent Gaussian increments. This yields [Brownian motion](../../../../../../../brownian-motion-split.md) itself.

## ↑ Ancestors (12)

1. [3](../3.md)
2. [C](../../c.md)
3. [1](../../../1.md)
4. [Paper 25](../../../../paper-25-split.md)
5. [Iii](../../../../split.md)
6. [2013](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
