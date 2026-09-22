<h1 id="4/solution">Solution</h1>

↑ **Parent:** [4](../4.md)

Set $Y_i=X_i^2$, $\overline Y=n^{-1}\sum_iY_i$ and $\tau^2=\operatorname{Var}_F(Y_1)=\mathbb E_FX_1^4-\theta^2$. The fourth-moment assumption makes $\tau^2$ finite, so the [variance of a sample mean](../../../../../variance-of-a-sample-mean.md) is $v=\tau^2/n$. Assume $n\geq2$, as required for leave-one-out estimation.

The [Jackknife variance estimator](../../../../../jackknife-variance-estimator.md) recomputes the original statistic on each sample with one observation removed. Here

$$
\widehat\theta_{(-i)}=\frac{n\overline Y-Y_i}{n-1},\qquad\overline\theta_J=\frac1n\sum_i\widehat\theta_{(-i)}=\overline Y.
$$

By the definition of the [Jackknife variance estimator](../../../../../jackknife-variance-estimator.md),

$$
\boxed{\widehat v_{\mathrm{JACK}}=\frac{n-1}{n}\sum_i(\widehat\theta_{(-i)}-\overline\theta_J)^2=\frac1{n(n-1)}\sum_i(Y_i-\overline Y)^2=\frac{s_Y^2}{n}.}
$$

For completeness, expanding the centered sum gives

$$
\mathbb E\sum_i(Y_i-\overline Y)^2=n\mathbb EY_1^2-n\mathbb E\overline Y^2=n(\tau^2+\theta^2)-n(\tau^2/n+\theta^2)=(n-1)\tau^2.
$$

Consequently $\mathbb E\widehat v_{\mathrm{JACK}}=\tau^2/n=v$. **The jackknife variance estimator is unbiased for this statistic.** This calculation uses only the finite fourth moment, not normality of the original observations.

Given the observed data, put $y_i=x_i^2$ and $\overline y=n^{-1}\sum_i y_i$. The [empirical distribution](../../../../../type-information-theory.md) assigns mass $1/n$ to each observed $x_i$, including repeated values with their multiplicities. A [bootstrap sample](../../../../../bootstrap-sample.md) consists of $n$ independent draws from this distribution, with replacement. The nonparametric bootstrap variance estimate is the conditional variance

$$
\widehat v_{\mathrm{BOOT}}=\operatorname{Var}_*\left(\frac1n\sum_{i=1}^n(X_i^*)^2\right).
$$

Independence of the bootstrap draws gives the exact [conditional bootstrap variance of a sample mean](../../../../../conditional-bootstrap-variance-of-a-sample-mean.md):

$$
\boxed{\widehat v_{\mathrm{BOOT}}=\frac1{n^2}\sum_i(y_i-\overline y)^2=\frac{n-1}{n}\widehat v_{\mathrm{JACK}}.}
$$

Thus its finite-sample expectation is $(n-1)v/n$, in contrast to the unbiased jackknife estimate. This is the [jackknife and bootstrap variance of a sample second moment](../../../../../jackknife-and-bootstrap-variance-of-a-sample-second-moment.md) scaling difference.

To approximate it by [Monte Carlo simulation](../../../../../monte-carlo-method.md), independently generate $B$ bootstrap samples. For replicate $b$, choose $n$ independent uniform indices $I_{b1},\ldots,I_{bn}\in\{1,\ldots,n\}$ and compute $T_b^*=n^{-1}\sum_jx_{I_{bj}}^2$. With $\overline T^*=B^{-1}\sum_bT_b^*$, use

$$
\widehat v_{\mathrm{BOOT},B}=\frac1{B-1}\sum_{b=1}^B(T_b^*-\overline T^*)^2.
$$

For $B>1$ this is conditionally unbiased for the bootstrap variance and converges to it as $B\to\infty$. Uniform indices can be obtained by $I=\lceil nU\rceil$ for uniforms on $(0,1]$.

Let $G_*(t)=P_*(T^*\leq t)$ be the conditional bootstrap distribution of the statistic. A nominal level $1-\alpha$ [percentile bootstrap confidence interval](../../../../../percentile-bootstrap-confidence-interval.md) is

$$
\boxed{[G_*^{-1}(\alpha/2),\ G_*^{-1}(1-\alpha/2)].}
$$

Reuse the bootstrap replicates, sort them as $T_{(1)}^*\leq\cdots\leq T_{(B)}^*$, and take the order statistics with ranks $\lceil B\alpha/2\rceil$ and $\lceil B(1-\alpha/2)\rceil$ as empirical quantiles. These are quantiles of the statistic itself, rather than reflected quantiles of its centered error. Increasing $B$ reduces simulation error; it does not turn an approximate [confidence interval](../../../../../confidence-interval.md) into an exact finite-sample one.

An analytic alternative follows from the [central limit theorem](../../../../../central-limit-theorem.md). If $\tau^2>0$, then $\sqrt n(\widehat\theta^n-\theta)\Rightarrow N(0,\tau^2)$, and the [sample variance](../../../../../sample-variance.md) $s_Y^2=(n-1)^{-1}\sum_i(x_i^2-\overline y)^2$ converges to $\tau^2$ by the [strong law of large numbers](../../../../../strong-law-of-large-numbers.md). The [Slutsky theorem](../../../../../slutsky-theorem.md) therefore gives the large-sample [normal approximation](../../../../../normal-approximation.md) interval

$$
\boxed{\left[\widehat\theta^n-z_{1-\alpha/2}\sqrt{\widehat v_{\mathrm{JACK}}},\ \widehat\theta^n+z_{1-\alpha/2}\sqrt{\widehat v_{\mathrm{JACK}}}\right],}
$$

where $z_{1-\alpha/2}$ is the [standard normal quantile](../../../../../standard-normal-quantile.md). Its lower endpoint may be truncated to zero because the parameter is nonnegative. If $\tau^2=0$, $X_i^2=\theta$ almost surely and the statistic identifies the parameter exactly; the interval degenerates to that value. The nondegenerate normal interval is asymptotic, not an exact Student interval under arbitrary $F$.

## ↑ Ancestors (10)

1. [4](../4.md)
2. [Paper 48](../../paper-48-split.md)
3. [Iii](../../split.md)
4. [2007](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
