<h1 id="3/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Principal component analysis](../../../../../../principal-component-analysis.md) replaces correlated measurements by uncorrelated linear compounds ordered by decreasing [variance](../../../../../../variance-split.md). Keeping the leading compounds gives a low-dimensional summary that preserves as much [variance](../../../../../../variance-split.md) as possible under orthonormal projection. It is an unsupervised description of variation, rather than a guarantee that the high-variance directions are best for classification or prediction.

Write $X_c=X-\mu$. For a unit loading vector $q$, the [variance](../../../../../../variance-split.md) of $q^TX_c$ is $q^T\Sigma q$. The [spectral theorem](../../../../../../spectral-theorem.md) gives an orthonormal eigenbasis $q_1,\ldots,q_p$ with [eigenvalues](../../../../../../eigenvalue.md) $\lambda_1\ge\cdots\ge\lambda_p\ge0$. If $q=\sum_jb_jq_j$ and $\sum_jb_j^2=1$, then

$$
q^T\Sigma q=\sum_j\lambda_jb_j^2\le\lambda_1.
$$

Equality is attained at $q_1$. Requiring the next loading to be orthogonal to the first excludes its eigendirection, so the same argument gives $q_2$ and [variance](../../../../../../variance-split.md) $\lambda_2$, and continues inductively. Repeated [eigenvalues](../../../../../../eigenvalue.md) permit any [orthonormal basis](../../../../../../orthonormal-basis.md) of the tied eigenspace. These are the [population principal components](../../../../../../population-principal-component.md).

With $Q=(q_1,\ldots,q_p)$, set $Y=Q^TX_c$. Then

$$
\boxed{\operatorname{Cov}(Y)=\Lambda=Q^T\Sigma Q
=\operatorname{diag}(\lambda_1,\ldots,\lambda_p),\qquad
\Sigma=Q\Lambda Q^T.}
$$

In particular the components are uncorrelated. They need not be independent unless, for example, $X$ is [multivariate normal](../../../../../../multivariate-normal-distribution.md). Finally

$$
\boxed{\sum_{j=1}^p\operatorname{Var}(Y_j)
=\sum_{j=1}^p\lambda_j
=\operatorname{tr}(\Sigma)
=\sum_{j=1}^p\operatorname{Var}(X_j).}
$$

The [trace](../../../../../../matrix-trace.md) equality follows from $Q^TQ=I$ and cyclicity of [trace](../../../../../../matrix-trace.md), so the rotation preserves total [variance](../../../../../../variance-split.md). The [explained variance of a principal component](../../../../../../explained-variance-of-a-principal-component.md) is its [eigenvalue](../../../../../../eigenvalue.md) divided by this total.

## ↑ Ancestors (11)

1. [A](../a.md)
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
