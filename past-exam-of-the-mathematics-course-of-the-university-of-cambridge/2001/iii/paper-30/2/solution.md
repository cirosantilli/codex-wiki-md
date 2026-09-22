<h1 id="2/solution">Solution</h1>

↑ **Parent:** [2](../2.md)

Treat the displayed entries as the lower triangle of a symmetric [sample covariance matrix](../../../../../sample-covariance-matrix.md) $S$, in the order mechanics, vectors, algebra, analysis, statistics. Compute the [precision matrix](../../../../../precision-matrix.md) $K=S^{-1}$. For a [multivariate normal distribution](../../../../../multivariate-normal-distribution.md), conditioning on all remaining coordinates gives

$$
\widehat{\operatorname{Var}}(Y_j\mid Y_{-j})=\frac1{K_{jj}},\qquad
\widehat{\operatorname{Corr}}(Y_i,Y_j\mid Y_{-(i,j)})
=-\frac{K_{ij}}{\sqrt{K_{ii}K_{jj}}}.
$$

These identities follow by fixing the other coordinates in the quadratic form of the normal density and completing the square. For the second identity, the conditional [precision matrix](../../../../../precision-matrix.md) for the retained pair is its $2\times2$ principal block; inverting that block gives the negative off-diagonal entry divided by the square root of the two diagonal entries.

Thus the two quantities to evaluate are

$$
\boxed{\frac1{K_{11}S_{11}}\simeq0.62,\qquad
-\frac{K_{54}}{\sqrt{K_{55}K_{44}}}\simeq0.25.}
$$

An equivalent procedure uses the [Schur complement covariance](../../../../../schur-complement-covariance.md): regress mechanics on the other four variables, or regress analysis and statistics separately on the remaining three. The first residual [variance](../../../../../variance-split.md) is $S_{11}-S_{1,-1}S_{-1,-1}^{-1}S_{-1,1}$; the second result is the [partial correlation](../../../../../partial-correlation.md) of the two residuals. No arithmetic is required to specify this method.

The model qualification is important: a covariance matrix alone determines linear-regression residual variances and [partial correlations](../../../../../partial-correlation.md). Identifying them with conditional quantities independent of the observed conditioning values uses the [multivariate normal](../../../../../multivariate-normal-distribution.md) model, or another model with the same conditional moments; it does not follow for arbitrary distributions.

## ↑ Ancestors (10)

1. [2](../2.md)
2. [Paper 30](../../paper-30-split.md)
3. [Iii](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
