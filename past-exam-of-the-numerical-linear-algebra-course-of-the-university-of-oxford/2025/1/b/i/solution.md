<h1 id="1/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Choose the nonnegative square roots of the [eigenvalues](../../../../../eigenvalue.md) of $A^TA$ for the diagonal entries of $\Sigma$, in nonincreasing order. Its assumed [matrix inverse](../../../../../matrix-inverse-split.md) exists, so these entries are positive. The [eigendecomposition](../../../../../spectral-decomposition.md) gives

$$
U^TU=\Sigma^{-1}V^TA^TAV\Sigma^{-1}
=\Sigma^{-1}\Sigma^2\Sigma^{-1}=I_n.
$$

Hence $U$ has [orthonormal](../../../../../orthonormal-set.md) columns. Also

$$
\boxed{U\Sigma V^T=AV\Sigma^{-1}\Sigma V^T=A}.
$$

Together with the [orthogonal matrix](../../../../../orthogonal-matrix.md) $V$ and the nonnegative [diagonal matrix](../../../../../diagonal-matrix.md) $\Sigma$, these are precisely the properties of a thin [singular value decomposition](../../../../../singular-value-decomposition.md).

## ↑ Ancestors (13)

1. [I](../i.md)
2. [B](../../b.md)
3. [1](../../../1.md)
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
