<h1 id="3/b/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Under [missing completely at random](../../../../../../../missing-completely-at-random.md), the observed second-year outcomes form a random subsample, so the direct pooled [complete-case analysis](../../../../../../../complete-case-analysis.md) estimate is

$$
\boxed{\widehat P_{\mathrm{CC}}(Y_2=1)=\frac{25}{65}=\frac5{13}\approx0.384615=38.46\%.}
$$

It is valid under [missing completely at random](../../../../../../../missing-completely-at-random.md) because dropout no longer changes the marginal distribution of second-year use. Pooling is simpler than reporting separate [conditional probabilities](../../../../../../../conditional-probability.md), but **MCAR alone does not make this estimate more efficient than the estimate in the previous part**. The fully observed first-year variable carries useful outcome information and can improve precision even when dropout is completely random.

To make the qualification explicit, write $X=Y_1$, $m(X)=P(Y_2=1\mid X)$, $\theta=E\{m(X)\}$ and $\rho=P(R=1)$ for the constant response [probability](../../../../../../../probability.md). For $N$ patients the leading [variance](../../../../../../../variance-split.md) of the pooled estimator is $\operatorname{Var}(Y_2)/(N\rho)$. The standardization estimator in the preceding part has leading [variance](../../../../../../../variance-split.md)

$$
V_{\mathrm{std}}=\frac1N\left[\operatorname{Var}\{m(X)\}+\frac{E\{m(X)(1-m(X))\}}{\rho}\right].
$$

Indeed its first-order centered contribution is $m(X)-\theta+R\{Y_2-m(X)\}/\rho$: the two terms have zero [covariance](../../../../../../../covariance.md), and their [variances](../../../../../../../variance-split.md) give that expression. The [law of total variance](../../../../../../../law-of-total-variance.md) therefore yields

$$
\boxed{V_{\mathrm{CC}}-V_{\mathrm{std}}=\frac{1-\rho}{N\rho}\operatorname{Var}\{m(X)\}\ge0.}
$$

The inequality is strict when there is dropout and first-year use predicts second-year use, as the distinct conditional rates suggest here. Thus the requested universal efficiency claim needs qualification. In the unrestricted joint binary-outcome model, maximizing the [observed-data likelihood](../../../../../../../observed-data-likelihood.md) under either [missing at random](../../../../../../../missing-at-random.md) or [missing completely at random](../../../../../../../missing-completely-at-random.md) gives the same standardization estimate $0.384889$: the all-patient first-year proportion and the two observed conditional second-year proportions maximize its factored outcome [likelihood](../../../../../../../likelihood-function.md). Restricting the distinct missingness parameters to a common response [probability](../../../../../../../probability.md) affects their factor, not this estimate. **The pooled value is the simple valid MCAR answer; retaining the first-year information gives the efficient MCAR answer and does not require replacing the previous estimate.**

## ↑ Ancestors (12)

1. [Iii](../iii.md)
2. [B](../../b.md)
3. [3](../../../3.md)
4. [Paper 32](../../../../paper-32-split.md)
5. [Iii](../../../../split.md)
6. [2014](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
