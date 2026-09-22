<h1 id="4/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

For the marginal mean model, $e^{\beta_0}$ is the expected term count for a student with all recorded covariates at their reference or zero values. If the treatment indicator is one for the new therapy and zero for the reference treatment, then $e^{\beta_1}$ is the ratio of population mean counts under the two treatments, holding the remaining covariates fixed. Values below one mean a reduced expected count; $100(1-e^{\beta_1})\%$ is the corresponding percentage reduction.

For the random-intercept model, $e^{\beta_0}$ is the conditional reference count at $b_i=0$, or multiplier $U_i=1$; the conditional baseline for student $i$ is $U_i e^{\beta_0}$. It is not automatically the mean-population baseline, which is $\tau e^{\beta_0}$. The conditional treatment [rate ratio](../../../../../../rate-ratio.md) for students with the same multiplier is $e^{\beta_1}$. Because the multiplier has the same distribution in the treatment groups and the mean uses a [logarithmic link function](../../../../../../logarithmic-link-function.md), that is also the marginal treatment [rate ratio](../../../../../../rate-ratio.md). This is the property that [marginal and conditional slopes agree for an independent log-link random intercept](../../../../../../marginal-and-conditional-slopes-agree-for-an-independent-log-link-random-intercept.md).

The parameter $\theta$ is the [variance](../../../../../../variance-split.md) of the positive student multiplier, not a Poisson sampling [variance](../../../../../../variance-split.md) or a treatment coefficient. Greater $\theta$ at fixed $\tau$ means greater heterogeneity in underlying propensity and larger between-term [covariance](../../../../../../covariance.md). Its extra contribution to the count [variance](../../../../../../variance-split.md) is $\theta a_{ij}^2$. If $\tau=1$ is imposed, $\theta$ is also the relative multiplier [variance](../../../../../../variance-split.md); otherwise the relative heterogeneity is $\theta/\tau^2$.

There is a necessary [identifiability](../../../../../../identifiability.md) qualification: if the multiplier mean $\tau$ is also unrestricted, [scale identifiability in a gamma random-intercept Poisson model](../../../../../../scale-identifiability-in-a-gamma-random-intercept-poisson-model.md) shows that replacing

$$
(U_i,\beta_0,\tau,\theta)\longmapsto
(cU_i,\beta_0-\log c,c\tau,c^2\theta)
$$

leaves the response law unchanged. Consequently only $\beta_0+\log\tau$ and $\theta/\tau^2$, together with the slopes, are identified from these counts without a scale convention. **Fixing the multiplier mean, usually to one, is needed to interpret the conditional intercept and heterogeneity scale separately**.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2002](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
