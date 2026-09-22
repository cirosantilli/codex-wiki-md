<h1 id="28j/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Multiplying the likelihood by the [gamma distribution](../../../../../../gamma-distribution.md) prior density gives

$$
\begin{aligned}
\pi(\theta\mid x_1,\ldots,x_n)
&\propto
\theta^n e^{-\theta S_n}
\theta^{\alpha-1}e^{-\beta\theta}\\
&=\theta^{\alpha+n-1}
e^{-(\beta+S_n)\theta}.
\end{aligned}
$$

Thus [Gamma-exponential conjugacy](../../../../../../gamma-exponential-conjugacy.md) gives

$$
\boxed{
\theta\mid X_1,\ldots,X_n
\sim\operatorname{Gamma}(\alpha+n,\beta+S_n),}
$$

where the second parameter is the rate. Under [squared-error loss](../../../../../../squared-error-loss.md), the [Bayes estimator under squared error loss](../../../../../../bayes-estimator-under-squared-error-loss.md) is the [posterior mean](../../../../../../posterior-mean.md), hence

$$
\boxed{
\widehat\theta_\pi
=\frac{\alpha+n}{\beta+S_n}.}
$$

## ↑ Ancestors (11)

1. [B](../b.md)
2. [28J](../../28j.md)
3. [Paper 3](../../../paper-3-split.md)
4. [Ii](../../../split.md)
5. [2019](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
