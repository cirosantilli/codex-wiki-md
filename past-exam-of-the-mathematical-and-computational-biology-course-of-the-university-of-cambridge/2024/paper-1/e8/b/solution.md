<h1 id="e8/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Place observations in rows of the data [matrix](../../../../../matrix.md) $X$. Since the coordinate [sample means](../../../../../sample-mean.md) are zero, the [Gram matrix](../../../../../gram-matrix.md) of its columns is

$$
X^TX=\begin{pmatrix}114&-48\\-48&86\end{pmatrix}.
$$

The [sample covariance matrix](../../../../../sample-covariance-matrix.md) is $S=X^TX/(3-1)$; using divisor three instead changes [eigenvalues](../../../../../eigenvalue.md) by a common factor and leaves [principal component loadings](../../../../../principal-component-loading.md) unchanged. For $X^TX$, the [characteristic polynomial](../../../../../characteristic-polynomial.md) is

$$
\det(X^TX-\lambda I)=(114-\lambda)(86-\lambda)-48^2
=\lambda^2-200\lambda+7500=(\lambda-150)(\lambda-50).
$$

For the larger [eigenvalue](../../../../../eigenvalue.md) $150$, the [eigenvector](../../../../../eigenvector.md) equation gives $-36\alpha-48\beta=0$, so $3\alpha+4\beta=0$. Normalize to unit [Euclidean norm](../../../../../euclidean-norm.md) and choose $v_1=(4/5,-3/5)^T$. An orthogonal unit [eigenvector](../../../../../eigenvector.md) for $50$ is $v_2=(3/5,4/5)^T$. Therefore

$$
\boxed{PC_1=\frac45x-\frac35y,\qquad PC_2=\frac35x+\frac45y}.
$$

The [sample variances](../../../../../sample-variance.md) of these [principal components](../../../../../principal-component.md) are $75$ and $25$, respectively. Their [principal component scores](../../../../../principal-component-score.md) for observations $A,B,C$ are

$$
\begin{array}{c|rr}
&PC_1&PC_2\\\hline
A&5&5\\
B&-10&0\\
C&5&-5
\end{array}.
$$

Either [eigenvector](../../../../../eigenvector.md) may be multiplied by $-1$ without changing its [principal component](../../../../../principal-component.md) direction or its [variance](../../../../../variance-split.md). No coordinate standardization is applied here: that would instead be [principal component analysis on a correlation matrix](../../../../../principal-component-analysis-on-a-correlation-matrix.md).

## ↑ Ancestors (13)

1. [B](../b.md)
2. [E8](../../e8.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2024](../../../split.md)
5. [Past exam of the mathematical and Computational Biology course of the University of Cambridge](../../../../split.md)
6. [Mathematical and Computational Biology course of the University of Cambridge](../../../../../mathematical-and-computational-biology-course-of-the-university-of-cambridge.md)
7. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
10. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
11. [University of Cambridge](../../../../../university-of-cambridge-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
