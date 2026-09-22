<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

A [Beta distribution](../../../../../../beta-distribution.md) is a convenient prior for a [probability](../../../../../../probability.md) $p\in(0,1)$ and is conjugate to the [binomial distribution](../../../../../../binomial-distribution.md) of the death count. Match its mean $m=0.05$ and [variance](../../../../../../variance-split.md) $v=0.02^2=0.0004$. For $p\sim\operatorname{Beta}(\alpha,\beta)$,

$$
\frac{\alpha}{\alpha+\beta}=m,\qquad
\frac{m(1-m)}{\alpha+\beta+1}=v.
$$

The [moment matching for a beta prior](../../../../../../moment-matching-for-a-beta-prior.md) formula gives

$$
\kappa=\alpha+\beta=\frac{0.05(0.95)}{0.0004}-1=117.75,
\qquad\boxed{\alpha=5.8875,\quad\beta=111.8625.}
$$

Conditional on $p$, use $D\sim\operatorname{Binomial}(90,p)$ and the observed count $D=9$. Multiplying its [likelihood](../../../../../../likelihood-function.md) $p^9(1-p)^{81}$ by the prior density gives the [Bayesian posterior](../../../../../../bayesian-posterior.md) through [Beta-binomial conjugacy](../../../../../../beta-binomial-conjugacy.md):

$$
\boxed{p\mid D=9\sim\operatorname{Beta}(14.8875,192.8625).}
$$

Under [squared-error loss](../../../../../../squared-error-loss.md), take its [posterior mean](../../../../../../posterior-mean.md) as the point estimate. A 95% equal-tail [credible interval](../../../../../../credible-interval.md) is given by its 0.025 and 0.975 quantiles. Numerically,

$$
\boxed{\widehat p_{\mathrm B}=0.07166,\qquad\operatorname{CI}_{0.95}=[0.04076,0.11035].}
$$

Matching two moments does not uniquely determine a prior distribution; the beta family is a justified convenient choice, not a conclusion forced by those moments. Its transfer to this hospital presumes that the historical between-hospital distribution is relevant to the present risk and [case mix](../../../../../../case-mix.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [4](../../4.md)
3. [Paper 29](../../../paper-29-split.md)
4. [Iii](../../../split.md)
5. [2001](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
