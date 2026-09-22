<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Principal component analysis](../../../../../../principal-component-analysis.md) replaces the original coordinates by orthogonal linear combinations, ordered so that the first few retain as much [variance](../../../../../../variance-split.md) as possible. It gives a lower-dimensional summary for visualization or compression and reveals the main directions of variation. A direction of large [variance](../../../../../../variance-split.md) need not be the direction most useful for classification.

Write $\mu=\mathbb EX$. For a unit vector $u$, the centered score $Y=u^T(X-\mu)$ has [variance](../../../../../../variance-split.md)

$$
\operatorname{Var}(Y)=u^T\Sigma u,\qquad u^Tu=1.
$$

Maximizing this [Rayleigh quotient](../../../../../../rayleigh-quotient.md) with a Lagrange multiplier gives

$$
\nabla_u\bigl[u^T\Sigma u-\lambda(u^Tu-1)\bigr]=2\Sigma u-2\lambda u=0.
$$

Thus a maximizing direction must be an [eigenvector](../../../../../../eigenvector.md) of the [covariance matrix](../../../../../../covariance-matrix.md). To identify the maximum, use the [spectral theorem for real symmetric matrices](../../../../../../spectral-theorem-for-real-symmetric-matrices.md) to choose an [orthonormal basis](../../../../../../orthonormal-basis.md) of [eigenvectors](../../../../../../eigenvector.md) $v_1,\ldots,v_p$, with [eigenvalues](../../../../../../eigenvalue.md) $\lambda_1\geq\cdots\geq\lambda_p\geq0$. Writing $u=\sum_jc_jv_j$ gives

$$
u^T\Sigma u=\sum_j\lambda_jc_j^2\leq\lambda_1\sum_jc_j^2=\lambda_1.
$$

Equality is attained at $u=v_1$. Consequently the first [population principal component](../../../../../../population-principal-component.md) is

$$
\boxed{Y_1=v_1^T(X-\mu),\qquad\operatorname{Var}(Y_1)=\lambda_1.}
$$

For each subsequent [principal component](../../../../../../principal-component.md), maximize the same [variance](../../../../../../variance-split.md) over unit coefficient vectors orthogonal to all the previously chosen ones. Restricting the expansion above to the remaining [eigenvectors](../../../../../../eigenvector.md) gives $v_2$, then $v_3$, and so on. Thus

$$
\boxed{Y_j=v_j^T(X-\mu),\qquad\operatorname{Cov}(Y_i,Y_j)=v_i^T\Sigma v_j=\lambda_j\mathbf1_{\{i=j\}}.}
$$

The [principal components](../../../../../../principal-component.md) are uncorrelated; they need not be independent unless additional distributional assumptions, such as joint Gaussianity, hold. Their total [variance](../../../../../../variance-split.md) is $\operatorname{tr}\Sigma=\sum_j\lambda_j$. Signs of [eigenvectors](../../../../../../eigenvector.md) are arbitrary, and a repeated [eigenvalue](../../../../../../eigenvalue.md) permits any [orthonormal basis](../../../../../../orthonormal-basis.md) in its eigenspace. In [sample principal component](../../../../../../sample-principal-component.md) calculations, replace $\mu$ by the [sample mean](../../../../../../sample-mean.md) and $\Sigma$ by the [sample covariance matrix](../../../../../../sample-covariance-matrix.md).

## ↑ Ancestors (11)

1. [A](../a.md)
2. [3](../../3.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
