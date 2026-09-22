<h1 id="19h/solution">Solution</h1>

↑ **Parent:** [19H](../19h.md)

Put $S=X_1+X_2+X_3$. Independence gives a [likelihood ratio](../../../../../likelihood-ratio.md)

$$
\frac{L(\theta_1)}{L(1)}=e^{-3(\theta_1-1)}\theta_1^S.
$$

Since $\theta_1>1$, this is strictly increasing in $S$. A threshold chosen between its values at $S=5$ and $S=6$ gives precisely the stated upper-tail critical region, so **it is a likelihood-ratio test**.

The sum has a [Poisson distribution](../../../../../poisson-distribution.md) with mean $3\theta$. Thus the [size of a statistical test](../../../../../size-of-a-statistical-test.md) and its [statistical power](../../../../../statistical-power.md) at $\theta_1$ are

$$
\boxed{\alpha=1-e^{-3}\sum_{j=0}^5\frac{3^j}{j!}=1-F_3(5)\simeq0.084,\qquad \operatorname{power}(\theta_1)=1-e^{-3\theta_1}\sum_{j=0}^5\frac{(3\theta_1)^j}{j!}.}
$$

For the grouped-area problem, let $S_1=\sum_{i=1}^mY_i$, $S_2=\sum_{i=m+1}^{2m}Y_i$, $T=S_1+S_2$. The null log likelihood, up to data-only constants, is

$$
\ell_0(\lambda)=-3ma\lambda+T\log\lambda+T\log a+S_2\log2.
$$

The [maximum-likelihood estimate](../../../../../maximum-likelihood-estimator.md) is $\widehat\lambda=T/(3ma)$, giving fitted means $T/(3m)$ and $2T/(3m)$ in the two groups. Under the alternative, the fitted group means are $\widehat\lambda_1=S_1/m$ and $\widehat\lambda_2=S_2/m$.

Use the increasing [generalized likelihood-ratio test](../../../../../generalized-likelihood-ratio-test.md) convention $\Lambda=\sup_{H_1}L/\sup_{H_0}L\geq1$, consistent with the printed positive $2\log\Lambda$. The exponential and factorial factors cancel, yielding the [likelihood-ratio test of area-proportional Poisson means](../../../../../likelihood-ratio-test-of-area-proportional-poisson-means.md)

$$
\boxed{\Lambda=\left(\frac{3S_1}{T}\right)^{S_1}\left(\frac{3S_2}{2T}\right)^{S_2},\qquad 2\log\Lambda=2\left[S_1\log\frac{3S_1}{T}+S_2\log\frac{3S_2}{2T}\right].}
$$

Terms with zero count are interpreted as $0\log0=0$; if $T=0$, take $\Lambda=1$. If the inverse ratio is used, the reported test statistic is instead $-2\log\Lambda$.

Under the null, the regular large-sample [Wilks theorem](../../../../../wilks-theorem.md) approximation is $2\log\Lambda\sim\chi^2_1$: the alternative has two rate parameters and the null one. The value $15.67$ far exceeds the usual $1\%$ critical value, about $6.63$, and has approximate tail probability $7.5\times10^{-5}$. Thus **reject proportionality of the expected counts to area**: the two groups show evidence of different territory densities. The statistic alone does not say which group has greater density; that requires $S_1/m$ versus $S_2/(2m)$. For small counts, an exact conditional test uses $S_1\mid T\sim\operatorname{Binomial}(T,1/3)$ under the null instead of the asymptotic calibration.

## ↑ Ancestors (10)

1. [19H](../19h.md)
2. [Paper 1](../../paper-1-split.md)
3. [Ib](../../split.md)
4. [2014](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
