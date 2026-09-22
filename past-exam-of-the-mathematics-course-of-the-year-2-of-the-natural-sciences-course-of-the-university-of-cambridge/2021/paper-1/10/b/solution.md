<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Fix one [self-adjoint](../../../../../self-adjoint-operator.md) choice of separated homogeneous [Dirichlet boundary conditions](../../../../../dirichlet-boundary-condition.md) or [Neumann boundary conditions](../../../../../neumann-boundary-condition.md) at each endpoint. The stated product condition then makes the boundary term $[awy y']_\alpha^\beta$ vanish. Multiplication of $Ly=\lambda wy$ by $y$ and [integration by parts](../../../../../integration-by-parts.md) give

$$
\lambda\int_\alpha^\beta wy^2dx=\int_\alpha^\beta yLy\,dx=\int_\alpha^\beta[aw(y')^2-wcy^2]dx.
$$

Hence define the [quadratic functionals](../../../../../quadratic-functional.md)

$$
\boxed{F[y]=\int_\alpha^\beta yLy\,dx=\int_\alpha^\beta[aw(y')^2-wcy^2]dx,\qquad G[y]=\int_\alpha^\beta wy^2dx,}
$$

and $\Lambda[y]=F[y]/G[y]$ for nonzero admissible $y$. The first expression for $F$ is linear in the operator $L$, and $G$ is linear in the weight $w$.

To prove the [minimum](../../../../../minimum-of-a-subset-of-a-total-order.md) statement, expand an admissible function in a complete weighted orthonormal system of [eigenfunctions](../../../../../eigenfunction.md) of the [Sturm-Liouville problem](../../../../../sturm-liouville-problem.md), $y=\sum_n c_ny_n$, with ordered [eigenvalues](../../../../../eigenvalue.md) $\lambda_0\leq\lambda_1\leq\cdots$. Self-adjointness and [orthogonality of Sturm-Liouville eigenfunctions](../../../../../orthogonality-of-sturm-liouville-eigenfunctions.md) give

$$
\Lambda[y]=\frac{\sum_n\lambda_n c_n^2}{\sum_n c_n^2}\geq\lambda_0.
$$

Equality is attained by a lowest [eigenfunction](../../../../../eigenfunction.md), so

$$
\boxed{\lambda_{\min}=\min_{y\ne0}\Lambda[y].}
$$

This is the [Rayleigh-Ritz variational principle](../../../../../rayleigh-ritz-variational-principle.md). The endpoint product condition is shorthand for fixed choices of boundary type: allowing each trial function to choose different endpoint types would not define one fixed [self-adjoint](../../../../../self-adjoint-operator.md) [eigenvalue](../../../../../eigenvalue.md) problem.

## ↑ Ancestors (13)

1. [B](../b.md)
2. [10](../../10.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2021](../../../split.md)
5. [Past exam of the mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../mathematics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
