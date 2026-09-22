<h1 id="6/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

By the [spectral theorem for real symmetric matrices](../../../../../spectral-theorem-for-real-symmetric-matrices.md), choose an [orthonormal eigenbasis](../../../../../orthonormal-eigenbasis.md) $\mathbf u_1,\mathbf u_2,\mathbf u_3$ corresponding to $6,\sqrt3,-\sqrt3$, with $\mathbf u_1=(1,1,1)^T/\sqrt3$. Write $P=[\mathbf u_1\ \mathbf u_2\ \mathbf u_3]$ and $\mathbf x=P\boldsymbol\xi$. This [orthogonal change of coordinates](../../../../../orthogonal-change-of-coordinates.md) gives

$$
\mathbf x^TM\mathbf x=6\xi_1^2+\sqrt3\xi_2^2-\sqrt3\xi_3^2,\qquad
x_1+x_2+x_3=\sqrt3\xi_1.
$$

The plane constraint is therefore $\xi_1=0$. On that plane the [quadratic form](../../../../../quadratic-form-split.md) vanishes exactly when

$$
\xi_2^2-\xi_3^2=(\xi_2-\xi_3)(\xi_2+\xi_3)=0.
$$

Consequently the entire set is

$$
\boxed{\{t(\mathbf u_2+\mathbf u_3):t\in\mathbb R\}
\ \cup\ \{t(\mathbf u_2-\mathbf u_3):t\in\mathbb R\}}.
$$

The two direction [vectors](../../../../../vector.md) are nonzero and not parallel, since $\mathbf u_2,\mathbf u_3$ are [linearly independent](../../../../../linear-independence.md). An invertible [orthogonal transformation](../../../../../orthogonal-transformation.md) maps each full line to a full line. Thus the set consists of precisely two infinite lines through the origin.

## ↑ Ancestors (13)

1. [C](../c.md)
2. [6](../../6.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2018](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
