<h1 id="2/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

In [Markov chain Monte Carlo](../../../../../../markov-chain-monte-carlo.md), retain the derived quantity $\delta=p_M-p_T$ at every iteration. Rough [BUGS](../../../../../../bugs.md) code using the actual observations is
```
model {
  pM ~ dbeta(0.5,0.5)
  pT ~ dbeta(0.5,0.5)
  milkAnswers ~ dbin(pM,4)
  teaAnswers ~ dbin(pT,4)
  delta <- pM-pT
  positive <- step(delta)
}
```
Supply `milkAnswers=3` and `teaAnswers=1`. Summarize `delta` by its [posterior mean](../../../../../../posterior-mean.md), empirical [quantiles](../../../../../../quantile-function.md) and [credible interval](../../../../../../credible-interval.md); the average of `positive` estimates $\mathbb P(p_M>p_T\mid\mathcal D)$. Here **$\mathbb E[\delta\mid\mathcal D]=0.4$**. Check [Markov chain Monte Carlo convergence diagnostics](../../../../../../markov-chain-monte-carlo-convergence-diagnostics.md) before interpreting the simulation. Since both [Bayesian posteriors](../../../../../../bayesian-posterior.md) are independent known [Beta distributions](../../../../../../beta-distribution.md), direct independent sampling is an equally valid, simpler way to obtain the same summaries.

## ↑ Ancestors (11)

1. [D](../d.md)
2. [2](../../2.md)
3. [Paper 35](../../../paper-35-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
