<h1 id="4/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Center time at 2008 by setting $s=t-4$, and initially ignore the explanatory covariates. A [Poisson generalized linear mixed model](../../../../../../poisson-generalized-linear-mixed-model.md) addressing both heterogeneity questions is

$$
Y_{it}\mid b_i\sim\operatorname{Poisson}\{P_{it}\exp(\beta_0+\beta_1s+b_{0i}+b_{1i}s)\},\qquad
\binom{b_{0i}}{b_{1i}}\sim N\left(0,
\begin{pmatrix}\tau_0^2&\tau_{01}\\\tau_{01}&\tau_1^2\end{pmatrix}\right).
$$

Here $\tau_0$ describes between-village variation of log rates in 2008, while $\tau_1$ describes heterogeneity of annual log-rate changes. The latent 2008 rate has median $e^{\beta_0}$, mean $e^{\beta_0+\tau_0^2/2}$ and coefficient of variation $\sqrt{e^{\tau_0^2}-1}$. A central 95% interval for latent village rates is $e^{\beta_0\pm1.96\tau_0}$; the corresponding interval for village-specific annual [rate ratios](../../../../../../rate-ratio.md) is $e^{\beta_1\pm1.96\tau_1}$. These describe heterogeneity, not confidence intervals for estimated fixed effects.

Fit an intercept-only random-effects model and then add a correlated [random slope](../../../../../../random-slope.md). Compare them with a [parametric bootstrap](../../../../../../parametric-bootstrap.md) of the likelihood improvement: the null slope variance is on the boundary, so an ordinary fixed-effect chi-squared reference is not automatically valid. Inspect uncertainty in both variance components, shrinkage of village-specific estimates, residual overdispersion and remaining serial correlation. A negative-binomial conditional model can distinguish additional within-village count variation from persistent village differences when the data support it.

By the [marginal mean of a Poisson random-slope model](../../../../../../marginal-mean-of-a-poisson-random-slope-model.md), the marginal log rate is $\beta_0+\beta_1s+(\tau_0^2+2s\tau_{01}+s^2\tau_1^2)/2$, so marginal curvature can arise even when each village has a straight conditional log trend. **Numerical variance estimates and evidence of heterogeneous slopes cannot be obtained for 32 villages from two displayed trajectories.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [4](../../4.md)
3. [Paper 102](../../../paper-102-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
