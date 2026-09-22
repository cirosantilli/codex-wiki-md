<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [ignorable missingness mechanism](../../../../../../ignorable-missingness-mechanism.md) need not be absent from the data-generating process. It means that [likelihood](../../../../../../likelihood-function.md) inference about the data-model parameters can omit the missingness factor, while still integrating over missing values.

Write the complete joint data [statistical probability density](../../../../../../probability-density-function.md) as $f_\theta(y,x)$ and the conditional missingness [probability](../../../../../../probability.md) as $g_\psi(r\mid y,x)$. All $y$ values and only $x_{\mathrm{obs}}$ are observed. Under [missing at random](../../../../../../missing-at-random.md), $g_\psi(r\mid y,x)$ is constant as $x_{\mathrm{mis}}$ varies with $(y,x_{\mathrm{obs}})$ fixed. The actual [observed-data likelihood](../../../../../../observed-data-likelihood.md) is therefore

$$
\begin{aligned}
L(\theta,\psi;y,x_{\mathrm{obs}},r)
 &=\int f_\theta(y,x_{\mathrm{obs}},x_{\mathrm{mis}})g_\psi(r\mid y,x_{\mathrm{obs}},x_{\mathrm{mis}})\,dx_{\mathrm{mis}}\\
 &=g_\psi(r\mid y,x_{\mathrm{obs}})\underbrace{\int f_\theta(y,x_{\mathrm{obs}},x_{\mathrm{mis}})\,dx_{\mathrm{mis}}}_{L_{\mathrm{obs}}(\theta;y,x_{\mathrm{obs}})}.
\end{aligned}
$$

The assumed distinctness is understood as independent variation of $\theta$ and $\psi$. Maximizing over $\psi$ multiplies $L_{\mathrm{obs}}$ by a factor independent of $\theta$; [likelihood ratios](../../../../../../likelihood-ratio.md), scores and [likelihood](../../../../../../likelihood-function.md) curvature for $\theta$ are therefore unchanged by omitting $g_\psi$. This proves [likelihood](../../../../../../likelihood-function.md) ignorability.

For implementation of the [observed-data likelihood with a missing covariate](../../../../../../observed-data-likelihood-with-a-missing-covariate.md), a [linear regression](../../../../../../linear-regression-split.md) model for $Y\mid X$ must be accompanied by an appropriate model for the distribution of $X$. For independent individuals, write $f_{\beta}(y\mid x)$ for the regression [statistical probability density](../../../../../../probability-density-function.md) and $g_\eta(x)$ for the age [statistical probability density](../../../../../../probability-density-function.md). Up to the ignorable factor,

$$
\boxed{L_{\mathrm{obs}}(\beta,\eta)=\prod_{i:R_i=1}f_\beta(y_i\mid x_i)g_\eta(x_i)\ \prod_{i:R_i=0}\int f_\beta(y_i\mid x)g_\eta(x)\,dx.}
$$

Ignorability does not authorize discarding missing-age cases or assuming their ages have the distribution seen in the complete cases. It removes the need to model the observation mechanism for [likelihood](../../../../../../likelihood-function.md) inference under the stated conditions, not the need to handle the missing covariates.

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 32](../../../paper-32-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
