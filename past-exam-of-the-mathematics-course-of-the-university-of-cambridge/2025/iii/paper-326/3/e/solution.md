<h1 id="3/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $(\sigma_j,u_j,v_j)$ be a singular system for $A$. The [Picard criterion](../../../../../../picard-criterion.md) for $f\in\operatorname{dom}(A^\dagger)$ is

$$
\sum_j\frac{|\langle f,v_j\rangle|^2}{\sigma_j^2}<\infty
$$

after discarding the component in $(\operatorname{ran}A)^\perp$. For $0<\tau<\|A\|^{-2}$, the partial series acts diagonally:

$$
Q_Nf
=\sum_j
\frac{1-(1-\tau\sigma_j^2)^{N+1}}{\sigma_j}
\langle f,v_j\rangle u_j.
$$

For each $j$ the multiplier in the numerator tends to one and lies in $[0,1]$. The Picard summability condition therefore supplies an $\ell^2$ dominating sequence, so the [dominated convergence theorem](../../../../../../dominated-convergence-theorem.md) gives

$$
\boxed{Q_Nf\longrightarrow
\sum_j\frac{\langle f,v_j\rangle}{\sigma_j}u_j
=A^\dagger f}.
$$

This is the series form of [Landweber iteration](../../../../../../landweber-iteration.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [3](../../3.md)
3. [Paper 326](../../../paper-326-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
