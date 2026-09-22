<h1 id="8d/solution">Solution</h1>

↑ **Parent:** [8D](../8d.md)

Write $Q=\sum_i(X_i-\bar X)^2$ and $Q_0=\sum_i(X_i-\mu_0)^2=Q+n(\bar X-\mu_0)^2$. The normal-sample likelihood is

$$
L(\mu,\sigma^2)=(2\pi\sigma^2)^{-n/2}\exp\left[-\frac{\sum_i(X_i-\mu)^2}{2\sigma^2}\right].
$$

Without the mean restriction, its maximum has $\widehat\mu=\bar X$ and $\widehat\sigma^2=Q/n$. Under the null, the maximizing variance is $Q_0/n$. Substituting them gives the [generalized likelihood-ratio test](../../../../../generalized-likelihood-ratio-test.md) statistic

$$
\Lambda=\frac{\sup_{H_0}L}{\sup L}=\left(\frac Q{Q_0}\right)^{n/2}=\boxed{\left(1+\frac{T^2}{n-1}\right)^{-n/2}},
$$

where $S^2=Q/(n-1)$ and $T=\sqrt n(\bar X-\mu_0)/S$. Assume $n\geq2$; $Q>0$ almost surely for positive population variance.

The ratio decreases strictly as $|T|$ increases, so rejecting for small $\Lambda$ is equivalent to rejecting for large $|T|$. Under $H_0$, $T$ has [Student's t-distribution](../../../../../student-s-t-distribution.md) with $n-1$ degrees of freedom. Therefore the exact size-$\alpha$ rule is

$$
\boxed{|T|>t_{n-1,\,1-\alpha/2}}.
$$

This is the two-sided [Student's t-test](../../../../../student-s-t-test.md). Equivalently reject when $\Lambda<(1+t_{n-1,1-\alpha/2}^2/(n-1))^{-n/2}$. No large-sample chi-squared approximation is needed for this [normal-mean likelihood ratio with unknown variance](../../../../../normal-mean-likelihood-ratio-with-unknown-variance.md).

## ↑ Ancestors (10)

1. [8D](../8d.md)
2. [Paper 3](../../paper-3-split.md)
3. [Ib](../../split.md)
4. [2005](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
