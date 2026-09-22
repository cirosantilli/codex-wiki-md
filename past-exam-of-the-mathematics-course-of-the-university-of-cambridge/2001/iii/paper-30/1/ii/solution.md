<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Under the diagonal covariance restriction, the [profile log-likelihood](../../../../../../profile-log-likelihood.md) separates into $p$ terms,

$$
-\frac n2\sum_j\left(\log v_j+\frac{S_{jj}}{v_j}\right)+C.
$$

Differentiating each term gives the restricted [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) $\widehat V_0=D=\operatorname{diag}(S_{11},\ldots,S_{pp})$. Both fitted trace terms equal $p$, so the [likelihood-ratio test statistic](../../../../../../likelihood-ratio-test-statistic.md) is

$$
\boxed{W=2\{\ell_p(S)-\ell_p(D)\}
=n\log\frac{\prod_jS_{jj}}{\det S}=-n\log\det R,}
$$

where $R=D^{-1/2}SD^{-1/2}$ is the [sample correlation matrix](../../../../../../sample-correlation-matrix.md). The statistic is nonnegative by the [Hadamard inequality](../../../../../../hadamard-determinant-inequality.md); large values indicate dependence. Equivalently, the likelihood ratio is $(\det S/\det D)^{n/2}$ and rejection is for small values of this ratio.

For fixed $p$ and a positive-definite true covariance, the [Wilks theorem](../../../../../../wilks-theorem.md) says that twice the maximized log-likelihood difference for nested regular models converges under the null to a [chi-squared distribution](../../../../../../chi-squared-distribution.md) with degrees of freedom equal to the dimension difference. The unrestricted covariance has $p(p+1)/2$ parameters and the restricted covariance has $p$; the unknown mean has the same $p$ parameters in both. Therefore the [Gaussian covariance diagonality likelihood-ratio test](../../../../../../gaussian-covariance-diagonality-likelihood-ratio-test.md) of asymptotic level $\alpha$ is

$$
\boxed{\text{reject if }W>\chi^2_{p(p-1)/2,\,1-\alpha}.}
$$

Within the [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md), diagonal covariance also means independent coordinates.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 30](../../../paper-30-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
