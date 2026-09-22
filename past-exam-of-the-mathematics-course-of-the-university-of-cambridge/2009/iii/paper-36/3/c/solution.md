<h1 id="3/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Centre and scale both predictors, particularly the raw dose whose scale is much larger than that of $\log(x_i+10)$. For example use $z_{1i}=[\log(x_i+10)-c_1]/s_1$, $z_{2i}=(x_i-c_2)/s_2$ and the [linear predictor](../../../../../../linear-predictor.md) $\eta_i=a_0+b_1z_{1i}+b_2z_{2i}$. This reduces the intercept-slope correlations and numerical scale disparities; further orthogonalizing correlated columns or updating coefficients jointly can improve [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) mixing. The exact old prior can be retained through the corresponding coefficient transformation; assigning new independent priors to transformed coefficients would instead change the prior.

For weakly informed plate effects or small $\tau$, use the [non-centred Gaussian random-effect parameterisation](../../../../../../non-centered-gaussian-random-effect-parameterization.md) $\lambda_{ij}=\tau z_{ij}$ with $z_{ij}\sim N(0,1)$. This often reduces dependence between the scale and local effects; it is not guaranteed to outperform the centred version when plate effects are strongly informed. Sensibly calibrated proper priors also avoid the enormous initial log intensities permitted by the stated coefficient ranges. Use dispersed chains and [Markov chain Monte Carlo convergence diagnostics](../../../../../../markov-chain-monte-carlo-convergence-diagnostics.md) to assess stationarity, agreement between chains and [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md). **Reparameterization can improve mixing; simply retaining more iterations does not remove poor mixing.**

## ↑ Ancestors (11)

1. [C](../c.md)
2. [3](../../3.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2009](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
