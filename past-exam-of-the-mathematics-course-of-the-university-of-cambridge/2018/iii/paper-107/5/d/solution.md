<h1 id="5/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Let $u=v+\psi$, so $v$ has zero [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md). Using the supplied form of the [minimal surface equation for a graph](../../../../../../minimal-surface-equation-for-a-graph.md), set

$$
Q_\psi(v)=\widetilde Q(v+\psi)-\widetilde Q(\psi),\qquad
f_\psi=\widetilde Q(\psi)-\Delta\psi.
$$

For $\|\psi\|_{C^{2,\alpha}}\leq\beta\leq1$ and $\|v\|,\|w\|\leq1$, the difference bound implies

$$
\|Q_\psi(v)\|_{C^{0,\alpha}}\leq C\|v\|_{C^{2,\alpha}}^2+2C\beta,
$$

and

$$
\|Q_\psi(v)-Q_\psi(w)\|_{C^{0,\alpha}}
\leq\bigl[C(\|v\|_{C^{2,\alpha}}+\|w\|_{C^{2,\alpha}})+2C\beta\bigr]\|v-w\|_{C^{2,\alpha}}.
$$

The shifted arguments stay in the permitted radius-two ball, and $\|f_\psi\|_{C^{0,\alpha}}\leq C\beta^2+C_n\beta$. The [Laplacian](../../../../../../laplacian.md) with zero [Dirichlet boundary condition](../../../../../../dirichlet-boundary-condition.md) has trivial [null space](../../../../../../kernel-of-a-linear-map.md) by the [maximum principle for harmonic functions](../../../../../../maximum-principle-for-harmonic-functions.md). Choose $\beta>0$ small enough that $2C\beta\leq\delta$ and $C\beta^2+C_n\beta\leq\varepsilon_0$, for the constants in part (c) with $L=\Delta$. Its [small-data existence for a nonlinear elliptic Dirichlet problem](../../../../../../small-data-existence-for-a-nonlinear-elliptic-dirichlet-problem.md) supplies $v$, and $\boxed{u=v+\psi}$ solves the [minimal surface equation for a graph](../../../../../../minimal-surface-equation-for-a-graph.md) with the required boundary values.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [5](../../5.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2018](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
