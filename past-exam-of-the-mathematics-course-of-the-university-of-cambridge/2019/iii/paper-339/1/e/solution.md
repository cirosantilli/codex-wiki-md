<h1 id="1/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Replace coordinate inequalities by the [Loewner order](../../../../../../loewner-order.md) and coordinate sums by [matrix trace](../../../../../../matrix-trace.md). The maximizing [semidefinite program](../../../../../../semidefinite-programming.md) is

$$
\boxed{F_k(X)=\max_{Y\in\mathbb S^n}\{\operatorname{tr}(XY):Y\succeq0,\ I-Y\succeq0,\ \operatorname{tr}Y=k\}.}
$$

Its feasible set is the [fantope](../../../../../../fantope.md). In an [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md) of $X$, its objective is $\sum_i\lambda_i(X)Y_{ii}$, and the diagonal entries of $Y$ belong to the [capped simplex](../../../../../../capped-simplex.md). Choosing $Y$ as the [orthogonal projection matrix](../../../../../../orthogonal-projection-matrix.md) onto the largest $k$ [eigenvectors](../../../../../../eigenvector.md) attains the [sum of the largest eigenvalues](../../../../../../sum-of-the-largest-eigenvalues.md), as in the [Ky Fan maximum principle](../../../../../../ky-fan-maximum-principle.md).

The minimizing [semidefinite program](../../../../../../semidefinite-programming.md) is

$$
\boxed{F_k(X)=\min_{t\in\mathbb R,\ S\in\mathbb S^n}\{kt+\operatorname{tr}S:S\succeq0,\ S+tI-X\succeq0\}.}
$$

For example, its [Lagrangian](../../../../../../lagrangian.md) arises by assigning $S\succeq0$ to $I-Y\succeq0$, keeping $Y\succeq0$ in the domain, and using free $t$ for $\operatorname{tr}Y=k$. Finiteness of the supremum over $Y$ requires $S+tI-X\succeq0$.

Equality follows directly by choosing $S$ to have [eigenvalues](../../../../../../eigenvalue.md) $(\lambda_i(X)-t)_+$ in the same [orthonormal eigenbasis](../../../../../../orthonormal-eigenbasis.md), with $t$ between the $k$th and $(k+1)$st [eigenvalues](../../../../../../eigenvalue.md), or below the smallest one for $k=n$. This is the [threshold semidefinite program for the largest eigenvalues](../../../../../../threshold-semidefinite-program-for-the-largest-eigenvalues.md), and it also verifies the endpoint case $k=n$.

## ↑ Ancestors (11)

1. [E](../e.md)
2. [1](../../1.md)
3. [Paper 339](../../../paper-339-split.md)
4. [Iii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
