<h1 id="3/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The given [equicorrelation covariance matrix](../../../../../../equicorrelation-covariance-matrix.md) can be written

$$
\Sigma=(1-r)I_4+r\mathbf1\mathbf1^T.
$$

On $\mathbf1=(1,1,1,1)^T$, the rank-one matrix $\mathbf1\mathbf1^T$ acts as multiplication by four. On the three-dimensional orthogonal complement $\{v:\sum_jv_j=0\}$ it acts as zero. Hence the [eigenvalues](../../../../../../eigenvalue.md) are **$1+3r$ and $1-r$ with multiplicity three**.

For $0<r<1$, the largest [eigenvalue](../../../../../../eigenvalue.md) is $1+3r$ and its normalized [eigenvector](../../../../../../eigenvector.md) is $\mathbf1/2$. Therefore the first [population principal component](../../../../../../population-principal-component.md) is

$$
\boxed{Y_1=\tfrac12\sum_{j=1}^4(X_j-\mu_j),\qquad
\operatorname{Var}(Y_1)=1+3r.}
$$

Omitting the centering merely changes the component by a constant and has no effect on its [variance](../../../../../../variance-split.md). Since $\operatorname{tr}\Sigma=4$, its explained fraction is

$$
\boxed{\frac{1+3r}{4}.}
$$

It rises from one quarter towards one as the positive common correlation increases. Outside the specified range, a valid covariance requires $-1/3\le r\le1$; for negative $r$ the sum direction is no longer the leading one.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [3](../../3.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
