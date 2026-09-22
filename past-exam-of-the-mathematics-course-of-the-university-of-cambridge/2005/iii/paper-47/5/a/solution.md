<h1 id="5/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Metropolis–Hastings algorithm](../../../../../../metropolis-hastings-algorithm.md) is useful when a target [posterior](../../../../../../bayesian-posterior.md) can be evaluated up to a [normalizing constant](../../../../../../normalizing-constant.md) but direct [independent](../../../../../../independent-random-variables.md) sampling or simple conditional sampling is unavailable. It constructs a [Markov chain](../../../../../../markov-chain.md) with that [posterior](../../../../../../bayesian-posterior.md) as invariant law. After adequate convergence, averages of functions of the chain estimate [posterior](../../../../../../bayesian-posterior.md) [expectations](../../../../../../expected-value.md), and the retained draws approximate marginal distributions, [quantiles](../../../../../../quantile-function.md) and credible intervals.

For the [Random-walk Metropolis algorithm](../../../../../../random-walk-metropolis-algorithm.md), at current $\theta$ propose $\theta'=\theta+Z$, where $Z$ has a symmetric distribution, often $N(0,\Sigma)$. With a symmetric proposal the acceptance [probability](../../../../../../probability.md) is

$$
\boxed{a(\theta,\theta')=\min\{1,\pi(\theta'\mid X)/\pi(\theta\mid X)\}.}
$$

Accept the proposal when an [independent](../../../../../../independent-random-variables.md) uniform is below this [probability](../../../../../../probability.md); otherwise retain the current value. For a nonsymmetric proposal $q(\theta'\mid\theta)$, include $q(\theta\mid\theta')/q(\theta'\mid\theta)$ in the ratio. [Detailed balance](../../../../../../detailed-balance.md) follows because the accepted flow is the minimum of the two proposed directional flows; rejection supplies the remaining self-transition [probability](../../../../../../probability.md). Irreducibility, appropriate recurrence and aperiodicity are also needed for convergence.

In the displayed [trace plots](../../../../../../trace-plot.md), the first parameter moves in small increments with pronounced long-term wandering and a shift from its early region to a later region. This is consistent with an undersized proposal or a strongly correlated slow direction. Measure its acceptance rate: if it is very high, increase that coordinate's proposal [variance](../../../../../../variance-split.md). The second parameter moves rapidly within regions but changes its level around iteration 4500; that is evidence against treating the full run as a settled stationary sample, and it suggests investigating dependence with the first parameter or separated [posterior](../../../../../../bayesian-posterior.md) regions. Its local scale may already be reasonable, so a blanket reduction of all proposal [variances](../../../../../../variance-split.md) would be unwarranted. The third parameter has conspicuous long plateaus, indicating many repeated states: if the recorded acceptance is low, reduce its proposal [variance](../../../../../../variance-split.md); also check constraints and dependence before deciding that scale alone is the cause.

**Rerun with coordinate-specific scale changes, inspect joint dependence, consider a covariance-based block proposal, and run longer chains from dispersed starting points.** The [MCMC trace diagnosis and proposal tuning](../../../../../../mcmc-trace-diagnosis-and-proposal-tuning.md) should include actual acceptance rates and effective sample sizes; the three marginal [trace plots](../../../../../../trace-plot.md) do not by themselves identify [correlations](../../../../../../pearson-correlation-coefficient.md) or prove convergence. Further practical details are in the three subparts.

## ↑ Ancestors (11)

1. [A](../a.md)
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
