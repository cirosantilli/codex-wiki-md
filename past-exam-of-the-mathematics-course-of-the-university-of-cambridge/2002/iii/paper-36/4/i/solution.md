<h1 id="4/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

The first approach specifies marginal means, [variances](../../../../../../variance-split.md) and an exchangeable correlation for each student's repeated counts. It is a moment model suitable for a [generalized estimating equation](../../../../../../generalized-estimating-equation.md); equality of the mean and [variance](../../../../../../variance-split.md) alone does not specify a full Poisson joint distribution. Different students supply [independent](../../../../../../independent-random-variables.md) sampling clusters, while the three counts within a student are dependent.

The second approach is a [Poisson generalized linear mixed model](../../../../../../poisson-generalized-linear-mixed-model.md) with a positive shared random multiplier $U_i=e^{b_i}$. Conditional on it, the three counts are [independent](../../../../../../independent-random-variables.md) Poisson variables; integrating over it gives a fully specified dependent joint law. The [gamma random-intercept Poisson model](../../../../../../gamma-random-intercept-poisson-model.md) uses Gamma shape $\tau^2/\theta$ and rate $\tau/\theta$, so $\mathbb E U_i=\tau$ and $\operatorname{Var}(U_i)=\theta$. Treat the covariates as fixed, with the same multiplier distribution across covariate/treatment groups, as required by this model.

Let $a_{ij}=\exp(\beta_0+\beta^{\mathsf T}x_{ij})$ and $m_{ij}=\mathbb E Y_{ij}$. The [law of total expectation](../../../../../../law-of-total-expectation.md), [law of total variance](../../../../../../law-of-total-variance.md) and [law of total covariance](../../../../../../law-of-total-covariance.md) give

$$
\boxed{m_{ij}=\tau a_{ij},\qquad
\operatorname{Var}(Y_{ij})=\tau a_{ij}+\theta a_{ij}^2,\qquad
\operatorname{Cov}(Y_{ij},Y_{ik})=\theta a_{ij}a_{ik}\quad(j\ne k)}.
$$

Thus each marginal is a [negative binomial distribution](../../../../../../negative-binomial-distribution.md) by the [Poisson-gamma mixture](../../../../../../poisson-gamma-mixture.md), rather than generally a Poisson variable. Put $\kappa=\theta/\tau^2$. Its [variance](../../../../../../variance-split.md) is $m_{ij}+\kappa m_{ij}^2$, and the marginal correlation is

$$
\boxed{\operatorname{Corr}(Y_{ij},Y_{ik})
=\frac{\kappa\sqrt{m_{ij}m_{ik}}}
{\sqrt{(1+\kappa m_{ij})(1+\kappa m_{ik})}}}.
$$

It is positive but usually depends on the two marginal means, so it need not be the common exchangeable correlation proposed in the first approach. The first method focuses on population mean effects with a chosen [working correlation matrix](../../../../../../working-correlation-matrix.md); the second models latent student heterogeneity and separates conditional Poisson variation from additional marginal variation. Correctly specified [likelihood](../../../../../../likelihood-function.md) inference for the second uses more distributional assumptions, while the first can retain valid mean inference despite a wrong working [covariance](../../../../../../covariance.md) by using a cluster-level sandwich [variance](../../../../../../variance-split.md).

## ↑ Ancestors (11)

1. [I](../i.md)
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
