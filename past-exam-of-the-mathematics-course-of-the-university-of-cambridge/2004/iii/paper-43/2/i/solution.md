<h1 id="2/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Use the usual [sample mean](../../../../../../sample-mean.md) and the divisor-$n-1$ [sample covariance matrix](../../../../../../sample-covariance-matrix.md),

$$
\bar x=\frac1n\sum_{j=1}^nx_j,\qquad S=\frac1{n-1}\sum_{j=1}^n(x_j-\bar x)(x_j-\bar x)^T.
$$

The residual sum is zero, so expanding $x_j-\mu=(x_j-\bar x)+(\bar x-\mu)$ gives

$$
\sum_j(x_j-\mu)(x_j-\mu)^T=(n-1)S+n(\bar x-\mu)(\bar x-\mu)^T.
$$

Multiplying the independent [multivariate normal densities](../../../../../../multivariate-normal-density.md) and taking logarithms yields the [log-likelihood](../../../../../../log-likelihood.md)

$$
\boxed{\ell(\mu,V)=-\frac{np}{2}\log(2\pi)-\frac n2\log|V|-\frac{n-1}{2}\operatorname{tr}(V^{-1}S)-\frac n2(\bar x-\mu)^TV^{-1}(\bar x-\mu).}
$$

Here $|V|$ is the [determinant](../../../../../../determinant.md) and $\operatorname{tr}$ denotes the [trace](../../../../../../matrix-trace.md). The [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md) are

$$
\boxed{\widehat\mu=\bar x,\qquad \widehat V=\frac{n-1}{n}S.}
$$

If $S$ instead denotes the divisor-$n$ [sample covariance matrix](../../../../../../sample-covariance-matrix.md), replace $(n-1)S$ by $nS$ and then $\widehat V=S$. These formulas describe a nonsingular [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) when the empirical scatter is [positive-definite](../../../../../../positive-definite-bilinear-form.md); if it is singular, there is no maximizer over positive-definite [covariance matrices](../../../../../../covariance-matrix.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [2](../../2.md)
3. [Paper 43](../../../paper-43-split.md)
4. [Iii](../../../split.md)
5. [2004](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
