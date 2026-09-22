<h1 id="7/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

Use the allowed ratio-of-expectations approximation where $G(u)>0$. The unconditional numerator and denominator from part (b) give

$$
\mathbb E\widehat H_{NA}(t)\approx\int_0^t\frac{G(u)\sum_iF_i(u)\,dH_i(u)}{G(u)\sum_iF_i(u)}=\int_0^t\frac{\sum_i e^{-H_i(u)}\,dH_i(u)}{\sum_i e^{-H_i(u)}}.
$$

The common censoring [survivor function](../../../../../../survival-function.md) cancels in this approximation. By differentiating the logarithm, its value is **the population integrated hazard**:

$$
\boxed{-\log\left(\frac1n\sum_{i=1}^n e^{-H_i(t)}\right)=\overline H(t).}
$$

This is not generally the arithmetic mean of the $H_i(t)$; it is the [cumulative hazard function](../../../../../../cumulative-hazard-function.md) of the population mixture from part (a). The cancellation requires a common independent censoring law and adequate observation of the time range.

**The approximation establishes approximate unbiasedness, not exact finite-sample unbiasedness.** For a direct counterexample, take one uncensored individual with [exponential distribution](../../../../../../exponential-distribution.md) of rate $\lambda$. The [Nelson–Aalen estimator](../../../../../../nelson-aalen-estimator.md) is then $\mathbf1_{T\le t}$, whose [expectation](../../../../../../expected-value.md) is $1-e^{-\lambda t}$, whereas $\overline H(t)=\lambda t$. Thus it is not an [unbiased estimator](../../../../../../unbiased-estimator.md) in general.

More explicitly, for independent individuals with a common event hazard $h$, the exact expected estimator is

$$
\mathbb E\widehat H_{NA}(t)=\int_0^t\mathbb P(Y(u)>0)h(u)\,du=\int_0^t\left[1-\{1-F(u)G(u)\}^n\right]h(u)\,du.
$$

This exhibits [finite-sample bias of Nelson–Aalen estimation](../../../../../../finite-sample-bias-of-nelson-aalen-estimation.md) and dependence on $G$ when empty [risk sets](../../../../../../risk-set.md) are possible. In a heterogeneous population, replacing the random ratios by ratios of their means introduces an additional approximation. On adequately observed intervals with large [risk sets](../../../../../../risk-set.md), the population-mixture expression is the appropriate large-sample target.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [7](../../7.md)
3. [Paper 207](../../../paper-207-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
