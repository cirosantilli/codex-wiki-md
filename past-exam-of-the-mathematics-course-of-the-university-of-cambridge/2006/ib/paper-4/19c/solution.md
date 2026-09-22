<h1 id="19c/solution">Solution</h1>

↑ **Parent:** [19C](../19c.md)

Write the common variance as $\sigma^2$. Independence and the [normal distribution](../../../../../normal-distribution.md) give

$$
\boxed{\bar X\sim N(\mu_X,\sigma^2/m),\qquad S_{XX}/\sigma^2\sim\chi^2_{m-1}.}
$$

Moreover $\bar X$ and $S_{XX}$ are independent. To see both assertions, standardize the observations into an isotropic Gaussian vector and choose an orthonormal basis with first vector $(1,\ldots,1)/\sqrt m$. Its first coordinate is $\sqrt m(\bar X-\mu_X)/\sigma$; the remaining independent standard normal coordinates have squared sum $S_{XX}/\sigma^2$. The same argument applies to the $Y$ sample, independently of the first sample.

Under the null hypothesis, the difference of sample means is $N(0,\sigma^2(1/m+1/n))$. The residual sums of squares add to an independent [chi-squared distribution](../../../../../chi-squared-distribution.md) with $\nu=m+n-2$ degrees of freedom. Define the [pooled sample variance](../../../../../pooled-sample-variance.md) and test statistic by

$$
S_p^2=\frac{S_{XX}+S_{YY}}{m+n-2},\qquad
\boxed{T=\frac{\bar X-\bar Y}{S_p\sqrt{1/m+1/n}}.}
$$

For $\nu>0$, under $H_0$ this is $Z/\sqrt{U/\nu}$ with independent $Z\sim N(0,1)$ and $U\sim\chi^2_\nu$. Hence **$T\sim t_{m+n-2}$ under the null**, the [Student t-distribution](../../../../../student-s-t-distribution.md).

Let $t_{\nu,0.99}$ be its 99th percentile. For the specified one-sided alternative, reject $H_0$ precisely when

$$
\boxed{T>t_{m+n-2,0.99}.}
$$

Because this distribution is continuous, the rejection probability under $H_0$ is exactly $0.01$, irrespective of the nuisance mean and variance. Large positive values supply evidence for $\mu_X>\mu_Y$; a two-sided or 0.995 cutoff would test a different alternative. The common-variance and independence assumptions are essential to this exact [Student t-test](../../../../../student-s-t-test.md). If both samples have size one, there are no residual degrees of freedom and the proposed unknown-variance test cannot be formed.

## ↑ Ancestors (10)

1. [19C](../19c.md)
2. [Paper 4](../../paper-4-split.md)
3. [Ib](../../split.md)
4. [2006](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
