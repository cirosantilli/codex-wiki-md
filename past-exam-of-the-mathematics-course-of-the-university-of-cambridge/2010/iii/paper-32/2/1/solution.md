<h1 id="2/1/solution">Solution</h1>

↑ **Parent:** [1](../1.md)

The [likelihood function](../../../../../../likelihood-function.md) for the shifted [exponential distribution](../../../../../../exponential-distribution.md) is

$$
L_n(\theta)=\exp\left(n\theta-\sum_{i=1}^nY_i\right)\mathbf1\{\theta\le Y_{(1)}\},\qquad Y_{(1)}=\min_iY_i.
$$

It increases strictly up to the smallest observation and is zero beyond it. Thus [shifted exponential maximum likelihood](../../../../../../shifted-exponential-maximum-likelihood.md) gives

$$
\boxed{\widehat\theta_n=Y_{(1)}.}
$$

For $t\ge0$, [independence](../../../../../../independent-random-variables.md) and the survival function of the [exponential distribution](../../../../../../exponential-distribution.md) give the exact [order statistic](../../../../../../order-statistic.md) law

$$
\mathbb P_\theta(\widehat\theta_n-\theta>t)=\prod_{i=1}^n\mathbb P_\theta(Y_i-\theta>t)=e^{-nt}.
$$

In particular, $\widehat\theta_n\ge\theta$ almost surely and $\mathbb P_\theta(|\widehat\theta_n-\theta|>\varepsilon)=e^{-n\varepsilon}\to0$. This proves [statistical consistency](../../../../../../consistency-statistics.md). The [exact endpoint limit for a shifted exponential distribution](../../../../../../exact-endpoint-limit-for-a-shifted-exponential-distribution.md) is stronger than an asymptotic approximation:

$$
\boxed{n(\widehat\theta_n-\theta)\sim\operatorname{Exp}(1)\ \text{for every }n,\qquad n(\widehat\theta_n-\theta)\xrightarrow{d}\operatorname{Exp}(1).}
$$

The limit is one-sided and nonnormal; the moving support endpoint explains why a regular square-root-$n$ [asymptotic normality of a maximum likelihood estimator](../../../../../../asymptotic-normality-of-a-maximum-likelihood-estimator.md) theorem does not apply here.

## ↑ Ancestors (11)

1. [1](../1.md)
2. [2](../../2.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
