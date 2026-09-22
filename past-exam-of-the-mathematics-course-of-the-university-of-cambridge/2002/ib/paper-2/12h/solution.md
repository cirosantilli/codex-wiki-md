<h1 id="12h/solution">Solution</h1>

↑ **Parent:** [12H](../12h.md)

For independent observations from a [normal distribution](../../../../../normal-distribution.md) with unknown mean and positive variance, the [maximum likelihood estimation](../../../../../maximum-likelihood-estimation.md) of the mean gives

$$
\boxed{\widehat\mu=\bar X=74.56}.
$$

Indeed $\sum_i(X_i-\mu)^2=S_{XX}+n(\bar X-\mu)^2$, which is minimized at $\mu=\bar X$. The [likelihood](../../../../../likelihood-function.md) is

$$
L(\mu,\sigma^2)=(2\pi\sigma^2)^{-n/2}\exp\!\left[-\frac{S_{XX}+n(\bar X-\mu)^2}{2\sigma^2}\right].
$$

For fixed $\mu$, differentiation in $\sigma^2$ gives the maximizer $[S_{XX}+n(\bar X-\mu)^2]/n$. Thus the unrestricted fit has $\widehat\sigma^2=S_{XX}/n$, whereas under the [null hypothesis](../../../../../null-hypothesis.md) $\mu=\mu_0$ the fitted variance is $[S_{XX}+n(\bar X-\mu_0)^2]/n$. Both maximize rather than minimize the likelihood: it tends to zero at either variance endpoint when the residual sum of squares is positive.

The restricted-to-unrestricted [likelihood ratio](../../../../../likelihood-ratio.md) is therefore

$$
\Lambda=\left[\frac{S_{XX}}{S_{XX}+n(\bar X-\mu_0)^2}\right]^{n/2}=\left(1+\frac{T^2}{n-1}\right)^{-n/2},\qquad T=\frac{\sqrt n(\bar X-\mu_0)}{s},\quad s^2=\frac{S_{XX}}{n-1}.
$$

The [generalized likelihood-ratio test](../../../../../generalized-likelihood-ratio-test.md) rejects for small $\Lambda$, equivalently large $|T|$. Under the null, $Z=\sqrt n(\bar X-\mu_0)/\sigma$ is standard normal, $U=S_{XX}/\sigma^2$ has a [chi-squared distribution](../../../../../chi-squared-distribution.md) with $n-1$ degrees of freedom, and they are independent. To see the independence, apply an [orthogonal matrix](../../../../../orthogonal-matrix.md) to the standardized normal sample, taking its first row to be $(1,\ldots,1)/\sqrt n$: the transformed coordinates remain independent standard normal variables, and $U$ is the sum of squares of the other $n-1$ coordinates. Hence $T=Z/\sqrt{U/(n-1)}$ has [Student's t-distribution](../../../../../student-s-t-distribution.md) with $n-1$ degrees of freedom.

For this two-sided test at $5\%$, the cutoff is the $97.5\%$ percentile of $t_9$, namely $2.26$. The data give

$$
s^2=\frac{12.824}{9},\qquad T=\frac{\sqrt{10}(74.56-75)}{\sqrt{12.824/9}}\simeq-1.166.
$$

Since $|T|<2.26$, **do not reject the manufacturer's mean-hardness claim at the $5\%$ level**. This is a failure to reject, not proof that the mean equals $75$.

## ↑ Ancestors (10)

1. [12H](../12h.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2002](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
