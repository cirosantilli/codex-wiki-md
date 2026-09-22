<h1 id="3/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Write $x=Q_ky$ and $\beta=\|b\|_2$. The [Arnoldi decomposition](../../../../../arnoldi-decomposition.md) and $b=\beta Q_{k+1}e_1$ give

$$
Ax-b=Q_{k+1}(\widetilde H_ky-\beta e_1).
$$

Because $Q_{k+1}$ has [orthonormal](../../../../../orthonormal-set.md) columns, it preserves the [Euclidean norm](../../../../../euclidean-norm.md). The [generalized minimal residual method](../../../../../generalized-minimal-residual-method.md) therefore reduces to the small [linear least-squares problem](../../../../../linear-least-squares-problem.md)

$$
\boxed{y_k=\underset{y\in\mathbb R^k}{\operatorname{argmin}}
\|\widetilde H_ky-\beta e_1\|_2,\qquad x_k=Q_ky_k}.
$$

Use [Givens rotations](../../../../../givens-rotation.md) on the [upper Hessenberg matrix](../../../../../upper-hessenberg-matrix.md) to obtain a [QR decomposition](../../../../../qr-decomposition.md)

$$
Z^T\widetilde H_k=\begin{pmatrix}R_k\\0\end{pmatrix},\qquad
g=Z^T(\beta e_1),
$$

where $Z$ is an [orthogonal matrix](../../../../../orthogonal-matrix.md) and $R_k$ is an [upper triangular matrix](../../../../../upper-triangular-matrix.md). Then solve $R_ky_k=g_{1:k}$ by [backward substitution in a triangular system](../../../../../backward-substitution-in-a-triangular-system.md) and form $Q_ky_k$. The resulting minimum [linear-system residual](../../../../../linear-system-residual.md) has [Euclidean norm](../../../../../euclidean-norm.md) $|g_{k+1}|$.

The small problem has a unique answer: if $\widetilde H_ky=0$, the [Arnoldi decomposition](../../../../../arnoldi-decomposition.md) gives $AQ_ky=0$. The [invertible matrix](../../../../../invertible-matrix.md) $A$ implies $Q_ky=0$, and the [orthonormality](../../../../../orthonormal-set.md) of $Q_k$ then gives $y=0$. Thus $\widetilde H_k$ has [full column rank](../../../../../full-column-rank.md) and $R_k$ is nonsingular.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [3](../../../3.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the numerical linear algebra course of the University of Oxford](../../../../split.md)
6. [Numerical linear algebra course of the University of Oxford](../../../../../numerical-linear-algebra-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
