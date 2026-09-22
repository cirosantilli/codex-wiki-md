<h1 id="12d/solution">Solution</h1>

↑ **Parent:** [12D](../12d.md)

For a [generalized likelihood-ratio test](../../../../../generalized-likelihood-ratio-test.md), maximize the [likelihood](../../../../../likelihood-function.md) separately over the null parameter space and the unrestricted space. Define $\Lambda=\sup_{H_0}L/\sup L\le1$, and reject for small $\Lambda$, equivalently large $T=-2\log\Lambda$. Choose the rejection threshold to achieve the desired null significance level, using an exact distribution when available or a justified asymptotic calibration; nuisance parameters are fitted under the respective restrictions.

For independent [Poisson distributions](../../../../../poisson-distribution.md), the likelihood is $L=\prod_i e^{-\lambda_i}\lambda_i^{X_i}/X_i!$. The unrestricted maximizers are $\widehat\lambda_i=X_i$, allowing zero as a boundary value. Under the common-mean null, maximizing $e^{-n\lambda}\lambda^{\sum_iX_i}$ gives $\widehat\lambda=\bar X$. The exponential and factorial factors cancel in the ratio, yielding

$$
\boxed{\Lambda=\prod_{i:X_i>0}\left(\frac{\bar X}{X_i}\right)^{X_i},\qquad T=-2\log\Lambda=2\sum_{i:X_i>0}X_i\log\frac{X_i}{\bar X}.}
$$

If all counts are zero, set $\Lambda=1$ and $T=0$; no division by $\bar X$ is then needed.

For positive $\bar X$, put $X_i=\bar X+\delta_i$, so $\sum_i\delta_i=0$. Expanding the logarithm gives

$$
(\bar X+\delta_i)\log(1+\delta_i/\bar X)=\delta_i+\frac{\delta_i^2}{2\bar X}+O(|\delta_i|^3/\bar X^2).
$$

Consequently

$$
\boxed{T=\frac1{\bar X}\sum_i(X_i-\bar X)^2+O\!\left(\frac{\sum_i|X_i-\bar X|^3}{\bar X^2}\right).}
$$

It is the [quadratic Pearson approximation to the Poisson deviance](../../../../../quadratic-pearson-approximation-to-the-poisson-deviance.md). The approximated statistic is the logarithmic ratio $T$, not the bounded raw ratio $\Lambda$.

Under the null in the large-common-count regime, this statistic has an approximate [chi-squared distribution](../../../../../chi-squared-distribution.md) with $n-1$ degrees of freedom: fitting the common mean removes one independent residual direction. For $n=7$, use six degrees of freedom. At $T=27.3$, the upper-tail probability in that approximation is

$$
P(\chi_6^2\ge27.3)=e^{-13.65}\left(1+13.65+\frac{13.65^2}{2}\right)\simeq1.27\times10^{-4}.
$$

Thus **reject the equal-mean null at conventional 5% or 1% significance levels**, provided the expected counts justify the chi-square approximation. No particular significance level or common count was supplied, so the numerical decision is stated with those assumptions.

## ↑ Ancestors (10)

1. [12D](../12d.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2001](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
