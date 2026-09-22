<h1 id="1/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let each observation have dimension $p$, and define the [sample mean](../../../../../../sample-mean.md) and the divisor-$n$ [sample covariance matrix](../../../../../../sample-covariance-matrix.md) by

$$
\bar y=\frac1n\sum_{i=1}^ny_i,\qquad S=\frac1n\sum_{i=1}^n(y_i-\bar y)(y_i-\bar y)^T.
$$

The [multivariate normal distribution](../../../../../../multivariate-normal-distribution.md) gives the [log-likelihood](../../../../../../log-likelihood.md)

$$
\ell(\mu,V)=-\frac{np}{2}\log(2\pi)-\frac n2\log\det V
-\frac12\sum_i(y_i-\mu)^TV^{-1}(y_i-\mu).
$$

Writing $y_i-\mu=(y_i-\bar y)+(\bar y-\mu)$ makes the cross terms vanish, and the last sum becomes $n\operatorname{tr}(V^{-1}S)+n(\bar y-\mu)^TV^{-1}(\bar y-\mu)$. Since $V$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), its minimum over the mean is at $\widehat\mu=\bar y$. Consequently

$$
\ell_p(V):=\max_\mu\ell(\mu,V)
=-\frac n2\log\det V-\frac n2\operatorname{tr}(V^{-1}S)+C.
$$

When $S$ is a [positive-definite matrix](../../../../../../positive-definite-matrix.md), $\log\det(V^{-1}S)=\log\det S-\log\det V$. Thus

$$
\ell_p(V)=\frac n2\log\det(V^{-1}S)-\frac n2\operatorname{tr}(V^{-1}S)+C',
$$

where $C'$ depends on the data but not on $V$.

For the [maximum-likelihood estimator](../../../../../../maximum-likelihood-estimator.md), consider the [positive-definite matrix](../../../../../../positive-definite-matrix.md) $Q=S^{1/2}V^{-1}S^{1/2}$, with positive [eigenvalues](../../../../../../eigenvalue.md) $a_1,\ldots,a_p$. The part of the [profile likelihood](../../../../../../profile-likelihood.md) depending on $V$ is $\frac n2\sum_j(\log a_j-a_j)$. The elementary inequality $\log a-a\leq-1$, with equality exactly at $a=1$, shows that the unique maximizing matrix is $Q=I$. Hence

$$
\boxed{\widehat\mu=\bar y,\qquad\widehat V=S.}
$$

The divisor is $n$, not the unbiased covariance divisor $n-1$. The regularity qualification matters: if $S$ is singular, the displayed logarithm of its determinant is not finite, and no positive-definite covariance maximizes the likelihood. Sending the fitted variance in a null direction of $S$ to zero makes the likelihood unbounded. For a nonsingular normal population, $S$ is positive definite almost surely when $n>p$, which is the setting of the large-sample test.

## ↑ Ancestors (11)

1. [I](../i.md)
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
