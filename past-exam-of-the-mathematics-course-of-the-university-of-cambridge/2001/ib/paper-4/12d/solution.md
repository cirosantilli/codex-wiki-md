<h1 id="12d/solution">Solution</h1>

↑ **Parent:** [12D](../12d.md)

Assume $n\ge2$ and $\sigma^2>0$. Up to a constant, the [log-likelihood](../../../../../log-likelihood.md) of the [normal sample](../../../../../normal-sample.md) is

$$
\ell(\mu,s)=-\frac n2\log s-\frac1{2s}\sum_i(X_i-\mu)^2,\qquad s=\sigma^2.
$$

For each $s$, the square is minimized at $\mu=\bar X$; optimizing the remaining one-variable likelihood gives the [maximum-likelihood estimators](../../../../../maximum-likelihood-estimator.md)

$$
\boxed{\widehat\mu=\bar X,\qquad
\widehat\sigma^2=\frac1n\sum_i(X_i-\bar X)^2.}
$$

They are the global maximum when the residual sum is positive, which occurs with probability one. On the exceptional all-equal sample the likelihood increases without bound as $s\downarrow0$.

To derive the distributions and independence, write $Z_i=(X_i-\mu)/\sigma$ and perform an orthogonal change of coordinates whose first row is $n^{-1/2}(1,\ldots,1)$. The transformed components $Z'_1,\ldots,Z'_n$ remain independent standard [normal random variables](../../../../../gaussian-random-variable.md), since their joint density depends only on the squared [Euclidean norm](../../../../../euclidean-norm.md). Then

$$
\widehat\mu=\mu+\frac{\sigma}{\sqrt n}Z'_1,
\qquad \frac{n\widehat\sigma^2}{\sigma^2}=\sum_{j=2}^n(Z'_j)^2.
$$

The first expression uses only $Z'_1$, the second only the other components. Consequently

$$
\boxed{\widehat\mu\sim N(\mu,\sigma^2/n),\qquad
n\widehat\sigma^2/\sigma^2\sim\chi^2_{n-1},\qquad
\widehat\mu\text{ and }\widehat\sigma^2\text{ are independent}.}
$$

This also exhibits why the maximum-likelihood variance uses divisor $n$, even though its chi-squared degrees of freedom are $n-1$.

The independent future observation satisfies $X_0-\bar X\sim N(0,\sigma^2(1+1/n))$. It is independent of the residual sum of squares, because both $X_0$ and $\bar X$ are independent of the residual vector. Combining this normal variable with the independent chi-squared variable gives

$$
T=\frac{X_0-\widehat\mu}{\widehat\sigma\sqrt{(n+1)/(n-1)}}\sim t_{n-1}.
$$

The event in the proposed [prediction interval](../../../../../prediction-interval.md) is equivalent to $|T|<\gamma\sqrt{(n-1)/n}$. By symmetry and continuity of [Student's t-distribution](../../../../../student-s-t-distribution.md), exact joint coverage $1-\alpha$ therefore requires

$$
\boxed{\gamma=\sqrt{\frac n{n-1}}\,t_{n-1,1-\alpha/2}.}
$$

This is the [normal prediction interval with maximum-likelihood variance](../../../../../normal-prediction-interval-with-maximum-likelihood-variance.md). The factor $\sqrt{n/(n-1)}$ cannot be dropped: the interval uses $\widehat\sigma$, not the unbiased residual standard deviation. Coverage here is over repeated joint sampling of the old and new observations, not a claim of parameter-free conditional coverage for every realized sample.

## ↑ Ancestors (10)

1. [12D](../12d.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
