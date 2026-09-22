<h1 id="4/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write $A_n=\max_{0\leq k<2^n}|\xi_{(k+1)2^{-n}}-\xi_{k2^{-n}}|$. The maximum of nonnegative numbers to the power $p$ is bounded by their sum, so the increment hypothesis gives

$$
\|A_n\|_p^p\leq\sum_{k=0}^{2^n-1}\mathbb E|\xi_{(k+1)2^{-n}}-\xi_{k2^{-n}}|^p
\leq C^p2^n2^{-np\beta}.
$$

Therefore $\|A_n\|_p\leq C2^{-n(\beta-1/p)}$. The [Minkowski inequality](../../../../../../minkowski-inequality.md) and completeness of $L^p$ imply convergence of the defining series whenever

$$
\boxed{0<\alpha<\beta-\frac1p,\qquad
\|K_\alpha\|_p\leq\frac{2C}{1-2^{-(\beta-1/p-\alpha)}}.}
$$

For a fully explicit argument, the norm of every tail is at most $2C\sum_{n\geq N}2^{-n(\beta-1/p-\alpha)}$, which tends to zero. Since the summands are nonnegative, their pointwise increasing sum equals this finite $L^p$ limit and is finite [almost surely](../../../../../../almost-sure-convergence.md). This is a guaranteed range; no endpoint convergence follows from the displayed summability estimate. The assumptions control increments only and do not require $\xi_0\in L^p$.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [4](../../4.md)
3. [Paper 201](../../../paper-201-split.md)
4. [Iii](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
