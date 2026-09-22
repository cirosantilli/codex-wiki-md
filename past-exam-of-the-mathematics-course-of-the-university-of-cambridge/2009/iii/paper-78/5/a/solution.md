<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

Use the [Euclidean norm](../../../../../../euclidean-norm.md) and its induced [operator norm](../../../../../../operator-norm.md). The [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) gives $\|A\|=\lambda_n$ and $\|A^{-1}\|=1/\lambda_1$. If $e=y_\delta-y$, then the direct inverse has error $A^{-1}e$, so

$$
\boxed{\|A^{-1}y_\delta-x\|\leq\frac\delta{\lambda_1}.}
$$

For nonzero $y$, the relation $\|y\|=\|Ax\|\leq\lambda_n\|x\|$ also gives

$$
\boxed{\frac{\|A^{-1}y_\delta-x\|}{\|x\|}\leq\kappa\frac\delta{\|y\|},\qquad\kappa=\frac{\lambda_n}{\lambda_1}.}
$$

This is the [spectral condition number of a positive-definite matrix](../../../../../../spectral-condition-number-of-a-positive-definite-matrix.md). The worst relative amplification is attained by exact data along an [eigenvector](../../../../../../eigenvector.md) for $\lambda_n$ and noise along one for $\lambda_1$. A large $\kappa$ therefore makes the reconstruction sensitive to relative data errors. Absolute sensitivity additionally depends on $\lambda_1$ itself: scaling every [eigenvalue](../../../../../../eigenvalue.md) equally leaves $\kappa$ unchanged but changes $1/\lambda_1$. Since the matrix is finite dimensional and positive definite, the inverse exists and is continuous; the issue is ill-conditioning rather than mathematical nonexistence or discontinuity.

## ↑ Ancestors (11)

1. [A](../a.md)
2. [5](../../5.md)
3. [Paper 78](../../../paper-78-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
