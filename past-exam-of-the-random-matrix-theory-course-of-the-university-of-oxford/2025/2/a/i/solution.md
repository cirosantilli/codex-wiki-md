<h1 id="2/a/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let $P$ be the $3$-by-$3$ evaluation [matrix](../../../../../matrix.md) $P_{i,\ell+1}=p_\ell(\lambda_i)$. The kernel evaluation [matrix](../../../../../matrix.md) is the [Gram matrix](../../../../../gram-matrix.md) $PP^T$, so [multiplicativity of the determinant](../../../../../multiplicativity-of-the-determinant.md) gives

$$
\det[K_3(\lambda_i,\lambda_j)]_{i,j=1}^3
=\det(PP^T)=(\det P)^2.
$$

Because the [polynomials](../../../../../polynomial-split.md) are [monic](../../../../../monic-polynomial.md) of consecutive degrees, their coefficient [matrix](../../../../../matrix.md) relative to $1,x,x^2$ is a [triangular matrix](../../../../../triangular-matrix.md) with unit diagonal. It has [determinant](../../../../../determinant.md) one, so the [Vandermonde determinant invariance under monic basis change](../../../../../vandermonde-determinant-invariance-under-monic-basis-change.md) gives

$$
\det P=\det\begin{pmatrix}
1&\lambda_1&\lambda_1^2\\
1&\lambda_2&\lambda_2^2\\
1&\lambda_3&\lambda_3^2
\end{pmatrix}
=\prod_{i<j}(\lambda_j-\lambda_i).
$$

Squaring removes the ordering sign. Thus the [Gaussian unitary ensemble](../../../../../gaussian-unitary-ensemble.md) [joint probability density function](../../../../../joint-probability-density.md) has precisely the kernel form

$$
\boxed{\rho_3(\boldsymbol\lambda)
=c_3\det[K_3(\lambda_i,\lambda_j)]_{i,j=1}^3
\exp\!\left(-\frac12\sum_i\lambda_i^2\right).}
$$

No [orthogonality](../../../../../orthogonal-vectors.md) of the [polynomials](../../../../../polynomial-split.md) is needed for this step.

## ↑ Ancestors (13)

1. [I](../i.md)
2. [A](../../a.md)
3. [2](../../../2.md)
4. [2025](../../../../2025-split.md)
5. [Past exam of the random matrix theory course of the University of Oxford](../../../../split.md)
6. [Random matrix theory course of the University of Oxford](../../../../../random-matrix-theory-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
