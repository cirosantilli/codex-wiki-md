<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Assume an independent Gaussian sample, positive-definite population covariance, and $n>p$. Define the [sample mean](../../../../../../sample-mean.md) and unbiased [sample covariance matrix](../../../../../../sample-covariance-matrix.md) by

$$
\bar X=\frac1n\sum_{i=1}^nX_i,\qquad S=\frac1{n-1}\sum_{i=1}^n(X_i-\bar X)(X_i-\bar X)^T.
$$

The standard test is based on [Hotelling's T-squared statistic](../../../../../../hotelling-s-t-squared-statistic.md)

$$
\boxed{T^2=n(\bar X-\mu_0)^TS^{-1}(\bar X-\mu_0).}
$$

Reject the [null hypothesis](../../../../../../null-hypothesis.md) for large values. Under the null its exact distribution is

$$
\boxed{\frac{n-p}{p(n-1)}T^2\sim F_{p,n-p}.}
$$

The factor uses the unbiased, divisor-$n-1$ covariance convention. Normal-sample theory makes $\bar X$ independent of the residual covariance, whose whitened version has a [Wishart distribution](../../../../../../wishart-distribution.md); this yields the stated [F-distribution](../../../../../../f-distribution.md). The condition $n>p$ gives invertibility of $S$ almost surely and positive denominator degrees of freedom.

This is also the [likelihood-ratio test](../../../../../../likelihood-ratio-test.md). To see the connection, put $W=(n-1)S$ and $\delta=\bar X-\mu_0$. The maximized covariance estimates under the unrestricted and null models are $W/n$ and $W/n+\delta\delta^T$, respectively. The determinant identity for a rank-one update gives

$$
\frac{|W/n+\delta\delta^T|}{|W/n|}=1+n\delta^TW^{-1}\delta=1+\frac{T^2}{n-1}.
$$

Thus the likelihood ratio is $(1+T^2/(n-1))^{-n/2}$, decreasing in $T^2$. The term best is understood here as this standard likelihood-ratio, affine-invariant procedure; a two-sided multidimensional alternative does not specify a single direction to optimize power against.

For the transformed sample $Y_i=AX_i+b$, with $A$ the prescribed nonsingular coordinate transformation, we have

$$
\bar Y-(A\mu_0+b)=A(\bar X-\mu_0),\qquad S_Y=ASA^T,\qquad S_Y^{-1}=A^{-T}S^{-1}A^{-1}.
$$

Consequently

$$
T_Y^2=n\delta^TA^T(A^{-T}S^{-1}A^{-1})A\delta=n\delta^TS^{-1}\delta=T_X^2.
$$

This proves the [affine invariance of Hotelling's statistic](../../../../../../affine-invariance-of-hotelling-s-statistic.md). **The statistic, its p-value and its test decision are unchanged by a nonsingular affine transformation**, provided the null mean is transformed with the data. Changes of units and rotations are included.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 46](../../../paper-46-split.md)
4. [Iii](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
