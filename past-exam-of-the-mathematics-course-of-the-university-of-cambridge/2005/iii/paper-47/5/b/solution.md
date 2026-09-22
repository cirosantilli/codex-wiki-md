<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For each observation time, use only the currently susceptible risk set $S_t$, with new-infection indicators $Y_{it}$. Put

$$
A_{it}(\beta)=\sum_{j\in I_t}d_{ij}^{-\beta},\qquad
L_1(\alpha,\beta)=\prod_t\prod_{i\in S_t}
(1-e^{-\alpha A_{it}(\beta)})^{Y_{it}}
e^{-\alpha A_{it}(\beta)(1-Y_{it})}.
$$

This is the [spatial Bernoulli infection model](../../../../../../spatial-bernoulli-infection-model.md), under [conditional independence](../../../../../../conditional-independence.md) of the indicators. Distances must be positive. Already infected trees should not be included as new susceptible trials. The minus sign in the power kernel is present in the original PDF, although it is absent in the converted TeX.

The parameter $\alpha$ must be nonnegative: for $\alpha<0$ and positive exposure, $1-e^{-\alpha A_{it}}<0$ is not a [probability](../../../../../../probability.md). Therefore the stated unrestricted normal [prior distribution](../../../../../../prior-probability.md) cannot literally define the model. A coherent interpretation is a normal [prior distribution](../../../../../../prior-probability.md) restricted to $\alpha>0$,

$$
p_\alpha^+(\alpha)=
\frac{\exp[-(\alpha-\mu_\alpha)^2/(2\sigma_\alpha^2)]}
{\sigma_\alpha\sqrt{2\pi}\,\Phi(\mu_\alpha/\sigma_\alpha)}
\mathbf1_{\{\alpha>0\}}.
$$

Here $\Phi$ is the [standard normal distribution](../../../../../../standard-normal-distribution.md) function. Use the same proper [prior distribution](../../../../../../prior-probability.md) in both kernel models. The given [Gaussian](../../../../../../normal-distribution.md) [prior distributions](../../../../../../prior-probability.md) for $\beta$ and $\gamma$ are mathematically valid on the real line for finite positive distances, though restricting them to positive values would impose decaying kernels and would require the corresponding normalized [prior distributions](../../../../../../prior-probability.md).

The full conditional kernels are

$$
\pi(\alpha\mid\beta,X)\propto p_\alpha^+(\alpha)L_1(\alpha,\beta),\qquad
\pi(\beta\mid\alpha,X)\propto
\exp[-(\beta-\mu_\beta)^2/(2\sigma_\beta^2)]L_1(\alpha,\beta).
$$

Neither is generally normal or another elementary conjugate family: the infection factors contain $1-e^{-\alpha A}$, and $A$ depends nonlinearly on $\beta$. Thus a simple conjugate [Gibbs sampler](../../../../../../gibbs-sampler.md) is unavailable. This does not make [Gibbs sampling](../../../../../../gibbs-sampler.md) logically impossible; exact rejection or slice conditional draws could be used if implemented. A straightforward alternative is [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) updates within each coordinate.

For example, put $\eta=\log\alpha$ and use symmetric [Gaussian](../../../../../../normal-distribution.md) random-walk proposals for $(\eta,\beta)$. The target in these coordinates is

$$
\widetilde\pi_1(\eta,\beta)\propto
L_1(e^\eta,\beta)p_\alpha^+(e^\eta)p_\beta(\beta)e^\eta.
$$

The factor $e^\eta$ is the [Jacobian determinant](../../../../../../jacobian-determinant.md) and must be retained. Accept according to the ratio of this target, either for a block or one coordinate at a time. [Posterior](../../../../../../bayesian-posterior.md) averages and [quantiles](../../../../../../quantile-function.md) of $e^\eta$ and $\beta$ estimate the requested marginal [posterior](../../../../../../bayesian-posterior.md) distributions.

To compare kernels, introduce $M\in\{1,2\}$ with positive model [prior distribution](../../../../../../prior-probability.md) [probabilities](../../../../../../probability.md) $w_1,w_2$. Under model two replace $A_{it}$ by $\sum_{j\in I_t}e^{-\gamma d_{ij}}$, defining $L_2(\alpha,\gamma)$. The joint model/parameter target is

$$
\pi(M,\alpha,\zeta\mid X)\propto
w_M L_M(\alpha,\zeta)p_\alpha^+(\alpha)p_M(\zeta),
$$

where $\zeta=\beta$ or $\gamma$ and $p_M$ is its normalized proper [prior distribution](../../../../../../prior-probability.md). Within each model use the preceding random-walk updates. For a concrete model switch, keep $\alpha$, propose the other model's kernel parameter independently from its [prior distribution](../../../../../../prior-probability.md), and use equal forward and reverse switch-selection [probabilities](../../../../../../probability.md). A move from $(1,\alpha,\beta)$ draws $\gamma\sim p_\gamma$ and has ratio

$$
\frac{w_2L_2(\alpha,\gamma)p_\gamma(\gamma)\,p_\beta(\beta)}
{w_1L_1(\alpha,\beta)p_\beta(\beta)\,p_\gamma(\gamma)}
=\boxed{\frac{w_2L_2(\alpha,\gamma)}{w_1L_1(\alpha,\beta)}}.
$$

Accept with the minimum of this ratio and one. The auxiliary-coordinate swap $(\alpha,\beta,\gamma)\mapsto(\alpha,\gamma,\beta)$ has absolute [Jacobian determinant](../../../../../../jacobian-determinant.md) one, so no additional factor occurs; unequal switch-selection [probabilities](../../../../../../probability.md) would require their reverse/forward ratio. This is a valid model-switching [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) construction even though the two active models have equal parameter dimension. [Prior distribution](../../../../../../prior-probability.md) proposals may be inefficient, so fitted proposals can be substituted provided their [probability densities](../../../../../../probability-density.md) remain in the acceptance ratio.

After checking mixing, estimate [posterior](../../../../../../bayesian-posterior.md) model [probabilities](../../../../../../probability.md) by the fractions of retained iterations in each model. The [Bayes factor](../../../../../../bayes-factor.md) in favor of the first kernel is

$$
\boxed{B_{12}=
\frac{\mathbb P(M=1\mid X)}{\mathbb P(M=2\mid X)}
\frac{w_2}{w_1}.}
$$

Use the [posterior](../../../../../../bayesian-posterior.md) distributions within each model as well as these odds to assess the competing distance kernels. Proper [prior distributions](../../../../../../prior-probability.md) and their model-dependent normalizing constants are essential for this comparison.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 47](../../../paper-47-split.md)
4. [Iii](../../../split.md)
5. [2005](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
