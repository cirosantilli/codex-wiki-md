<h1 id="18h/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The joint mass factorizes through $T=\sum_iX_i$, so $T$ is sufficient for $q$. If $\lambda=\sqrt q$, then

$$
E[X_1^2-X_1]=E[X_1(X_1-1)]=\lambda^2=q.
$$

Conditionally on $T$, $X_1\sim\operatorname{Bin}(T,1/n)$. Rao–Blackwell therefore gives the unbiased estimator

$$
E[X_1(X_1-1)\mid T]=\frac{T(T-1)}{n^2}.
$$

For $n\ge2$ the original estimator is not a [function](../../../../../../function-split.md) of $T$, so the variance reduction is strict.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [18H](../../18h.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ib](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
