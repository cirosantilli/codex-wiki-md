<h1 id="1/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

With the divisor-$n$ [sample covariance matrix](../../../../../../sample-covariance-matrix.md) defined above, the [maximum-likelihood estimators](../../../../../../maximum-likelihood-estimator.md) are

$$
\boxed{\widehat\mu=\bar x,\qquad \widehat V=S.}
$$

Their joint [sampling distribution](../../../../../../sampling-distribution.md) is specified by

$$
\boxed{\bar X\sim N_p(\mu,V/n),\qquad nS\sim W_p(n-1,V),
\qquad\bar X\ \text{and}\ S\ \text{are independent}.}
$$

Here $W_p(\nu,V)$ uses the [Wishart distribution](../../../../../../wishart-distribution.md) convention $\mathbb E W=\nu V$. Thus the covariance [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md) has [expected value](../../../../../../expected-value.md) $(n-1)V/n$; the [unbiased estimator](../../../../../../unbiased-estimator.md) of the [covariance matrix](../../../../../../covariance-matrix.md) is $nS/(n-1)$. These distributions follow from [orthogonal projections](../../../../../../orthogonal-projection.md) of the jointly [multivariate normal](../../../../../../multivariate-normal-distribution.md) observations onto the constant-observation direction and its [orthogonal complement](../../../../../../orthogonal-complement.md), though no proof is required here. The covariance maximum in the positive-definite parameter space requires $S$ nonsingular, which holds almost surely when $n>p$ and $V$ is positive definite. Otherwise the [rank of a centered sample covariance matrix](../../../../../../rank-of-a-centered-sample-covariance-matrix.md) shows why the usual unrestricted finite maximum does not exist.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [1](../../1.md)
3. [Paper 42](../../../paper-42-split.md)
4. [Iii](../../../split.md)
5. [2003](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
