<h1 id="11b/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The identity follows immediately from the product rule:

$$
\nabla\cdot(\kappa\psi\nabla\phi)
=\psi\nabla\cdot(\kappa\nabla\phi)+\kappa\nabla\psi\cdot\nabla\phi.
$$

If $\phi_1,\phi_2$ have the same boundary data, put $\psi=\phi_1-\phi_2$. Integrating the identity with $\phi=\psi$ gives

$$
\int_V\kappa|\nabla\psi|^2dV=0
$$

because the volume equation and boundary term vanish. Positivity of $\kappa$ makes $\psi$ constant, and its boundary value makes it zero, proving uniqueness.

For any $w=\phi+\psi$ with $\psi=0$ on the boundary, expansion gives

$$
\int\kappa|\nabla w|^2
=\int\kappa|\nabla\phi|^2+int\kappa|\nabla\psi|^2,
$$

because the cross term vanishes by the same integration by parts. This proves the inequality and the [Dirichlet principle](../../../../../../dirichlet-principle.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [11B](../../11b.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ia](../../../split.md)
5. [2023](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
