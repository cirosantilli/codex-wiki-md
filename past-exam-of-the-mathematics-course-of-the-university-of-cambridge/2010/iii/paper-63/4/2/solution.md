<h1 id="4/2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Let $\ell_j(\tau)=\prod_{k\ne j}(\tau-c_k)/(c_j-c_k)$ be the [Lagrange interpolation](../../../../../../lagrange-polynomial.md) basis. Set $Y_i=P(t_n+c_i h)$ and $F_j=f(t_n+c_jh,Y_j)$. Since $P'$ is a [polynomial](../../../../../../polynomial-split.md) of degree at most $s-1$, the collocation conditions give

$$
P'(t_n+\tau h)=\sum_{j=1}^s\ell_j(\tau)F_j.
$$

Integrate from zero to $c_i$ and to one to obtain

$$
Y_i=y_n+h\sum_j a_{ij}F_j,\qquad
y_{n+1}=y_n+h\sum_jb_jF_j,
$$



$$
\boxed{a_{ij}=\int_0^{c_i}\ell_j(\tau)d\tau,\qquad
b_j=\int_0^1\ell_j(\tau)d\tau.}
$$

These are the stage and update equations of a [Runge-Kutta method](../../../../../../runge-kutta-method.md) with nodes $c_i$. Conversely, stages satisfying these equations reconstruct $P$ by integrating the displayed interpolation [polynomial](../../../../../../polynomial-split.md), so the equivalence works in both directions. Because $\sum_j\ell_j=1$, they also satisfy the [collocation tableau row-sum identity](../../../../../../collocation-tableau-row-sum-identity.md) $\sum_j a_{ij}=c_i$.

## ↑ Ancestors (11)

1. [2](../2.md)
2. [4](../../4.md)
3. [Paper 63](../../../paper-63-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
