<h1 id="3/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

For admissible data, the [Moore–Penrose inverse of an operator](../../../../../../moore-penrose-inverse-of-an-operator.md) selects the [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md):

$$
\boxed{x^\dagger\in(\ker A)^\perp,\qquad \|Ax^\dagger-y\|=\inf_{x\in X}\|Ax-y\|,\qquad A^\dagger y=x^\dagger.}
$$

Its domain is $\operatorname{ran}A\oplus(\operatorname{ran}A)^\perp$. When the equation is consistent it is the solution of $Ax=y$ orthogonal to the kernel; for inconsistent admissible data it solves the [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md) and projects away the component orthogonal to the range.

Take a [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md) satisfying $Av_j=\sigma_ju_j$, $A^*u_j=\sigma_jv_j$. The generalized inverse is

$$
\boxed{x^\dagger=\sum_j\frac{\langle y,u_j\rangle}{\sigma_j}v_j.}
$$

The [Picard criterion](../../../../../../picard-criterion.md) requires the squared coefficients to be summable. For an infinite-rank compact operator, $\sigma_j\to0$, so $\|A^\dagger u_j\|=1/\sigma_j\to\infty$ even though $\|u_j\|=1$. Hence $A^\dagger$ is unbounded. Finite-rank compact operators do not have this obstruction. Data failing the Picard condition need not have a least-squares minimizer at all, even when the infimum residual is zero.

## ↑ Ancestors (11)

1. [I](../i.md)
2. [3](../../3.md)
3. [Paper 335](../../../paper-335-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
