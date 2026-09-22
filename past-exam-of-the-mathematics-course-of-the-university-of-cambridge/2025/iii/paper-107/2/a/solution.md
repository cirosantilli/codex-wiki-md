<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Write the flux as

$$
A^i(x,z,\eta)=a^{ij}(x,z,\eta)\eta_j.
$$

After expanding the [divergence](../../../../../../divergence.md), the [principal symbol of a partial differential equation](../../../../../../principal-symbol-of-a-partial-differential-equation.md) along a candidate solution $u$ is determined by

$$
A^{ik}(x,u,Du)=\frac{\partial A^i}{\partial\eta_k}
=a^{ik}+\frac{\partial a^{ij}}{\partial\eta_k}D_ju.
$$

Only the symmetric part $A_s=(A+A^T)/2$ contributes to $A^{ik}D_{ik}u$. The problem is elliptic along $u$ when $\xi^TA_s\xi\geq0$ for every $\xi$, and it is strictly elliptic where this quantity is positive for every nonzero $\xi$. It is uniformly elliptic on a set when constants $0<\lambda\leq\Lambda<\infty$, independent of the point, satisfy

$$
\lambda|\xi|^2\leq\xi^TA_s(x,u,Du)\xi\leq\Lambda|\xi|^2.
$$

These definitions separate pointwise positive definiteness from a quantitative lower and upper bound; a [degenerate elliptic operator](../../../../../../degenerate-elliptic-operator.md) may lose strict ellipticity at some jets.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 107](../../../paper-107-split.md)
4. [Iii](../../../split.md)
5. [2025](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
