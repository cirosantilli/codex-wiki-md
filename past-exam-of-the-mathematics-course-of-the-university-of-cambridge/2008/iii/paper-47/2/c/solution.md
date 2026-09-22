<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [composition of absolutely summable time-series filters](../../../../../../composition-of-absolutely-summable-time-series-filters.md) is $(1-B^{12})(1-B)$, with $B$ the [backshift operator](../../../../../../backshift-operator.md). Thus

$$
\boxed{Z_t=X_t-X_{t-1}-X_{t-12}+X_{t-13},}
$$

and its only nonzero coefficients are $c_0=1$, $c_1=-1$, $c_{12}=-1$, $c_{13}=1$. Multiplication of the two [filter gains](../../../../../../filter-gain.md) gives

$$
\boxed{G_c(\lambda)=4\sin(\lambda/2)|\sin(6\lambda)|,\quad0\leq\lambda\leq\pi.}
$$

Equivalently, its [spectral density transformation under a linear filter](../../../../../../spectral-density-transformation-under-a-linear-filter.md) is $f_Z=16\sin^2(\lambda/2)\sin^2(6\lambda)f_X$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2008](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
