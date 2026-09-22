<h1 id="19h/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For a target $a(\theta)$, the [bias](../../../../../../bias-of-an-estimator.md) of an integrable [estimator](../../../../../../estimator.md) $T$ is $\mathbb E_\theta T-a(\theta)$; it is an [unbiased estimator](../../../../../../unbiased-estimator.md) if this is zero at every allowed parameter value. Here $Y$ has a [zero-truncated Poisson distribution](../../../../../../zero-truncated-poisson-distribution.md), $\theta>0$, and $p=1-e^{-\theta}\in(0,1)$. Write an estimator based only on $Y$ as $t(Y)$, assuming a finite expectation for every $\theta>0$. Unbiasedness requires

$$
\sum_{y=1}^\infty t(y)\frac{\theta^y}{y!}=(e^\theta-1)(1-e^{-\theta})=e^\theta+e^{-\theta}-2.
$$

Absolute integrability at every positive parameter ensures that the power series on the left converges absolutely on every complex disc. Uniqueness of coefficients in a [power series](../../../../../../power-series.md) therefore gives $t(y)=0$ for odd $y$ and $t(y)=2$ for positive even $y$. Conversely these values give the displayed identity, so

$$
\boxed{T=2\mathbf1_{\{Y\text{ even}\}}}
$$

is the unique [unbiased estimator](../../../../../../unbiased-estimator.md) of this form. The uniqueness claim concerns nonrandomized functions of $Y$; allowing external randomness would permit addition of independent mean-zero noise.

For this [parity estimator for a zero-truncated Poisson count](../../../../../../parity-estimator-for-a-zero-truncated-poisson-count.md), usefulness depends on the loss, but under [squared-error loss](../../../../../../squared-error-loss.md) it performs poorly despite being an [unbiased estimator](../../../../../../unbiased-estimator.md). Since $\mathbb P(Y\text{ even})=p/2$, $\mathbb E T^2=2p$ and

$$
\operatorname{Var}T=2p-p^2=1-e^{-2\theta}.
$$

It takes the inadmissible value $2$ with positive probability, and its [variance](../../../../../../variance-split.md) tends to one rather than zero as $\theta\to\infty$. Clipping to the parameter interval gives $T_c=\min(T,1)=\mathbf1_{\{Y\text{ even}\}}$. This has [bias](../../../../../../bias-of-an-estimator.md) $-p/2$, but

$$
\mathbb E[(T_c-p)^2]=p/2<2p-p^2=\mathbb E[(T-p)^2],\qquad0<p<1.
$$

Thus a simple biased [estimator](../../../../../../estimator.md) strictly improves its [mean squared error](../../../../../../mean-squared-error.md) at every parameter value; uniqueness among unbiased estimators does not make it optimal for this loss.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [19H](../../19h.md)
3. [Paper 1](../../../paper-1-split.md)
4. [Ib](../../../split.md)
5. [2017](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
