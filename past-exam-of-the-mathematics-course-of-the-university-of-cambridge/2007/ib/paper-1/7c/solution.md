<h1 id="7c/solution">Solution</h1>

↑ **Parent:** [7C](../7c.md)

Write $\bar X=n^{-1}\sum_iX_i$, $Q=\sum_i(X_i-\bar X)^2$, and $Q_0=\sum_i(X_i-\mu_0)^2=Q+n(\bar X-\mu_0)^2$. The normal [likelihood](../../../../../likelihood-function.md) is proportional to $(\sigma^2)^{-n/2}\exp[-\sum_i(X_i-\mu)^2/(2\sigma^2)]$. Its unrestricted maximizers are $\widehat\mu=\bar X$, $\widehat\sigma^2=Q/n$. Under the null the [variance](../../../../../variance-split.md) maximizer is $Q_0/n$. Substitution gives the [generalized likelihood-ratio test](../../../../../generalized-likelihood-ratio-test.md) statistic

$$
\Lambda=\left(\frac Q{Q_0}\right)^{n/2}
=\left(1+\frac{T^2}{n-1}\right)^{-n/2},\qquad
T=\frac{\sqrt n(\bar X-\mu_0)}S,\quad S^2=\frac Q{n-1}.
$$

The ratio decreases as $|T|$ increases, so the likelihood-ratio rejection region is two-sided in $T$. Under $H_0$, $\sqrt n(\bar X-\mu_0)/\sigma$ is standard normal and $Q/\sigma^2$ is independent chi-squared with $n-1$ degrees of freedom. Independence follows by resolving the isotropic Gaussian sample vector into its projection on the constant vector and its orthogonal complement. Hence $T$ has the exact [Student t-distribution](../../../../../student-s-t-distribution.md) with $n-1$ degrees of freedom.

For a chosen [significance level](../../../../../significance-level.md) $\alpha$, compute the [sample mean](../../../../../sample-mean.md) and the sample [standard deviation](../../../../../standard-deviation.md) with denominator $n-1$, and **reject precisely when**

$$
\boxed{|T|>t_{n-1,\,1-\alpha/2}.}
$$

Equivalently, report the two-sided $p$-value $2[1-F_{t_{n-1}}(|T|)]$. This requires $n\geq2$ and positive population [variance](../../../../../variance-split.md); $S>0$ holds almost surely under that model. The nuisance [variance](../../../../../variance-split.md) is removed by the exact null distribution, so one should not substitute a normal critical value or a large-sample chi-squared approximation. This is the [normal-mean likelihood ratio with unknown variance](../../../../../normal-mean-likelihood-ratio-with-unknown-variance.md).

## ↑ Ancestors (10)

1. [7C](../7c.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
