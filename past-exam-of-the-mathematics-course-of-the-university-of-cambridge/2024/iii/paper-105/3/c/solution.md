<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Put

$$
D=\|\psi_0\|_{H^1(U)}+\|\psi_1\|_{L^2(U)}.
$$

The assumed [energy estimate](../../../../../../energy-estimate.md) for the linear [wave equation](../../../../../../wave-equation-split.md) and the first nonlinear estimate give, for $w\in X_{b,\tau}$,

$$
\|Aw\|_{X_\tau}
\leq C_0\left(D+\beta\tau^{1/2}b^2\right).
$$

Choose $b\geq2C_0D$ and then choose $\tau>0$ so small that $C_0\beta\tau^{1/2}b^2\leq b/2$. Then $A$ maps the closed ball $X_{b,\tau}$ into itself.

For $w,\widetilde w\in X_{b,\tau}$, the difference $Aw-A\widetilde w$ solves the linear equation with zero [Cauchy data](../../../../../../cauchy-data.md) and forcing $F(w)-F(\widetilde w)$. The second nonlinear estimate therefore gives

$$
\|Aw-A\widetilde w\|_{X_\tau}
\leq2C_0\gamma\tau^{1/2}(b+b^2)
\|w-\widetilde w\|_{X_\tau}.
$$

Shrinking $\tau$ once more makes the coefficient strictly smaller than one. Since $X_\tau$ is a [Banach space](../../../../../../banach-space-split.md) and its closed ball is complete, $A$ is a contraction on $X_{b,\tau}$.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 105](../../../paper-105-split.md)
4. [Iii](../../../split.md)
5. [2024](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
