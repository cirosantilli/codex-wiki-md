<h1 id="5/ii/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For conditional individual response profiles use a [logistic random-intercept model for repeated binary outcomes](../../../../../../../logistic-random-intercept-model-for-repeated-binary-outcomes.md). Introduce a subject effect $B_i\sim N(0,\tau^2)$ independently across subjects and independently of treatment and baseline [covariates](../../../../../../../covariate.md), under the specified model. Conditional on $B_i,z_i,x_i$, assume the three responses are independent [Bernoulli random variables](../../../../../../../bernoulli-distribution.md) with

$$
p_{ij}(b)=P(Y_{ij}=1\mid B_i=b,z_i,x_i),\qquad \operatorname{logit}p_{ij}(b)=\alpha_C+\phi_C z_i+\beta_C^Tx_i+\delta_C t_j+b.
$$

Here $B_i$ is persistent unmeasured subject heterogeneity and $\tau^2$ its [variance](../../../../../../../variance-split.md). It induces dependence after integration: for distinct visits, the response [covariance](../../../../../../../covariance.md) is $\operatorname{Cov}_B(p_{ij}(B),p_{ik}(B))$, generally positive. This is a complete joint [generalized linear mixed model](../../../../../../../generalized-linear-mixed-model.md), unlike a mean-only [GEE](../../../../../../../generalized-estimating-equation.md) specification.

Under [missing at random](../../../../../../../missing-at-random.md) conditional on the observed responses and baseline variables, with [distinct parameters](../../../../../../../distinct-parameters.md) for missingness and outcomes, the missingness model is ignorable for likelihood inference. Let $\mathcal O_i=\{j:R_{ij}=1\}$. The outcome [observed-data likelihood](../../../../../../../observed-data-likelihood.md) is

$$
L(\gamma_C,\tau^2)=\prod_i\int_{-\infty}^{\infty}\prod_{j\in\mathcal O_i}p_{ij}(b)^{y_{ij}}[1-p_{ij}(b)]^{1-y_{ij}}\frac{e^{-b^2/(2\tau^2)}}{\sqrt{2\pi\tau^2}}\,db.
$$

The omitted Bernoulli factors sum to one over missing outcomes. Fit the fixed coefficients and $\tau^2$ by maximizing this integrated [likelihood](../../../../../../../likelihood-function.md), with suitable quadrature or another justified integration method. If $\tau=0$, use the limiting point-mass model. Correct response and random-effect distributions, identifiable coefficients and regularity are needed; the latent distribution assumption is not merely a convenient working covariance.

For patient $i$, combine the fitted model with the posterior density of $B_i$ proportional to its normal density times that patient's observed Bernoulli factors. Integrating $p_{ij}(b)$ over this posterior gives a patient-specific predicted response profile. The treatment [odds ratio](../../../../../../../odds-ratio.md) for a fixed $b$ and the same baseline variables is $e^{\phi_C}$. This conditional contrast does not by itself identify each person's unobserved causal treatment effect: a parallel-arm trial observes only one treatment per person. Random slopes or heterogeneous treatment effects require further modelling and sufficient information; they are not implied by fitting a [random intercept](../../../../../../../random-intercept.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [Ii](../../ii.md)
3. [5](../../../5.md)
4. [Paper 38](../../../../paper-38-split.md)
5. [Iii](../../../../split.md)
6. [2003](../../../../../split.md)
7. [Past exam of the mathematics course of the University of Cambridge](../../../../../../split.md)
8. [Mathematics course of the University of Cambridge](../../../../../../../mathematics-course-of-the-university-of-cambridge.md)
9. [Course of the University of Cambridge](../../../../../../../course-of-the-university-of-cambridge.md)
10. [University of Cambridge](../../../../../../../university-of-cambridge-split.md)
11. [List of universities](../../../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../../../split.md)
