<h1 id="4/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Center the log-time predictor and the baseline log measurement near their sample means, so the intercept describes a typical predictor configuration. This reduces intercept-slope posterior correlation and can improve [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md) mixing. If exactly the original model is required, transform the intercept prior consistently when changing coordinates rather than silently assigning a different independent prior.

For weakly informed child effects, a [non-centered Gaussian random-effect parameterization](../../../../../../non-centered-gaussian-random-effect-parameterization.md) can also help:

$$
z_i\sim N(0,1),\qquad\boxed{\alpha_i=\delta+\tau z_i.}
$$

This retains the same conditional [prior distribution](../../../../../../prior-probability.md) for $\alpha_i$ but removes its prior-scale dependence from the sampled $z_i$. It can reduce strong dependence between the effects and $\tau$. A centered parameterization can be better when each child's effect is very accurately observed, so improvement is not automatic. Blocking strongly correlated coefficients is another option. Check the resulting chains with [Markov chain Monte Carlo convergence diagnostics](../../../../../../markov-chain-monte-carlo-convergence-diagnostics.md) and [effective sample size of a Markov chain](../../../../../../effective-sample-size-of-a-markov-chain.md), rather than judging convergence from the number of iterations alone.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [4](../../4.md)
3. [Paper 36](../../../paper-36-split.md)
4. [Iii](../../../split.md)
5. [2010](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
