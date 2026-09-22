<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

For noisy data, exact equality $Ax=y$ may be impossible: the data can have a component outside the [operator range](../../../../../../range-of-a-bounded-linear-operator.md). A [least-squares solution of a linear inverse problem](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) instead minimizes

$$
 J(x)=\frac12\|Ax-y\|_Y^2.
$$

For any variation $h\in X$, the [adjoint operator](../../../../../../adjoint-operator.md) gives

$$
 DJ(x)[h]=\operatorname{Re}\langle Ax-y,Ah\rangle_Y
 =\operatorname{Re}\langle A^*(Ax-y),h\rangle_X.
$$

Thus [statistical homogeneity](../../../../../../statistical-homogeneity.md) in every direction is the [normal equation for a linear inverse problem](../../../../../../normal-equation-for-a-linear-inverse-problem.md), $A^*Ax=A^*y$. It is also sufficient for a global minimum: when it holds,

$$
\boxed{J(x+h)-J(x)=\frac12\|Ah\|_Y^2\geq0.}
$$

The residual is orthogonal to the closure of the range, since it lies in $\ker A^*$. A normal-equation solution therefore fits the component of the data representable by the forward map, while leaving the perpendicular component unfitted. If there is more than one such solution, select the [minimum-norm least-squares solution](../../../../../../minimum-norm-least-squares-solution.md), which lies in $(\ker A)^\perp$.

These facts explain the formulation, but do not make the inverse problem well posed. A [compact operator](../../../../../../compact-operator-split.md) of infinite rank typically has nonclosed [operator range](../../../../../../range-of-a-bounded-linear-operator.md), so even the least-squares infimum need not be attained. A [least-squares solution](../../../../../../least-squares-solution-of-a-linear-inverse-problem.md) exists exactly when the [orthogonal projection](../../../../../../orthogonal-projection.md) of $y$ onto $\overline{\operatorname{Ran}A}$ belongs to $\operatorname{Ran}A$. In a [singular system of a compact operator](../../../../../../singular-system-of-a-compact-operator.md), this becomes the [Picard criterion](../../../../../../picard-criterion.md). Also, the nonzero [eigenvalues](../../../../../../eigenvalue.md) of $A^*A$ are the squares of the [singular values](../../../../../../singular-value.md) of $A$: solving the [operator normal equation](../../../../../../normal-equation-for-a-linear-inverse-problem.md) directly can worsen numerical conditioning. **The [operator normal equation](../../../../../../normal-equation-for-a-linear-inverse-problem.md) expresses least squares; it does not itself regularize the inverse problem.** The subsequent finite [Landweber iteration](../../../../../../landweber-iteration.md) and its stopping rule provide the [inverse-problem regularization](../../../../../../regularization-of-an-inverse-problem.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 76](../../../paper-76-split.md)
4. [Iii](../../../split.md)
5. [2015](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
