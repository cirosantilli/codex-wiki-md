<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Use the [continuous semimartingale decomposition](../../../../../../continuous-semimartingale-decomposition.md) $X=X_0+M+A$, where $M$ is a continuous local martingale and $A$ is a continuous adapted [finite-variation process](../../../../../../finite-variation-process.md). Pointwise limits preserve predictability, so $H$ is predictable; it is bounded by the common bound for the $H_n$.

Localize so that $[M]_\infty$ and the total variation $V(A)_\infty$ are bounded. The [Doob L2 maximal inequality](../../../../../../doob-l2-maximal-inequality.md) and the [Itô isometry](../../../../../../ito-isometry.md) give

$$
\mathbb E\sup_t\left|\int_0^t(H_n-H)\,dM\right|^2
\leq4\mathbb E\int_0^\infty(H_n-H)^2\,d[M]
\longrightarrow0
$$

by the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md). For the finite-variation part,

$$
\sup_t\left|\int_0^t(H_n-H)\,dA\right|
\leq\int_0^\infty|H_n-H|\,dV(A)
\longrightarrow0
$$

almost surely, again by dominated convergence, now for each sample path. Hence the two integrals converge uniformly in probability after every localization. Part (b) removes the localization and proves

$$
\int H_n\,dX\longrightarrow\int H\,dX
$$

u.c.p.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [2](../../2.md)
3. [Paper 202](../../../paper-202-split.md)
4. [Iii](../../../split.md)
5. [2026](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
