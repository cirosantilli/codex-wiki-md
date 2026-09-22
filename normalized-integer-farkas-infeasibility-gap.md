# Normalized integer Farkas infeasibility gap

↑ **Parent:** [Farkas certificate for linear inequalities](farkas-certificate-for-linear-inequalities.md)

Suppose $A,b$ have integer entries of absolute value at most $U\geq1$, $A$ has $n$ columns, and $Ax\geq b$ is infeasible. A [Farkas certificate for linear inequalities](farkas-certificate-for-linear-inequalities.md) can be chosen with $\lambda\geq0$, $A^T\lambda=0$, $\mathbf1^T\lambda=1$ and the displayed lower bound. Normalize an infeasibility certificate to obtain the last equality, then maximize $b^T\lambda$ over the resulting compact [linear polyhedron](linear-polyhedron.md). A maximizing [extreme point](extreme-point.md) has at most $n+1$ positive entries: otherwise the augmented columns $(A_i^T,1)$ on its support would be dependent, allowing feasible perturbations in both directions. For its $k\leq n+1$ independent supported columns, select $k$ independent equations. [Cramer's rule](cramer-s-rule.md) expresses the supported entries with a common nonzero integer determinant denominator. That determinant has absolute value at most $k!U^k\leq[(n+1)U]^{n+1}$. The positive value $b^T\lambda$ therefore has a positive integer numerator over a denominator of at most this size, proving the bound.

## ↑ Ancestors (8)

1. [Farkas certificate for linear inequalities](farkas-certificate-for-linear-inequalities.md)
2. [Farkas' lemma](farkas-lemma.md)
3. [Conic optimization](conic-optimization.md)
4. [Convex optimization](convex-optimization-split.md)
5. [Mathematical optimization](mathematical-optimization-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Full-dimensional relaxation of integer inequalities](full-dimensional-relaxation-of-integer-inequalities.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-34/2/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2003/iii/paper-37/2/solution.md)
