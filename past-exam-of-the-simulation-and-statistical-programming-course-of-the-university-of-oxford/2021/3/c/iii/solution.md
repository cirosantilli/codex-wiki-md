<h1 id="3/c/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Use several complementary [Markov chain Monte Carlo convergence diagnostics](../../../../../markov-chain-monte-carlo-convergence-diagnostics.md), monitoring both $p$ and $\beta$ rather than judging the chain solely by its length:

- [Trace plots](../../../../../trace-plot.md) of each parameter and the [log-posterior](../../../../../log-posterior.md) against iteration, including early iterations and later windows. Look for initial drift, long flat stretches, abrupt switches and sustained changes in spread. Several [independent](../../../../../independent-random-variables.md) chains started at dispersed points should explore the same region after [burn-in](../../../../../burn-in.md).
- Plots of cumulative [sample means](../../../../../sample-mean.md) and selected [sample quantiles](../../../../../sample-quantile.md) against iteration. Compare chains and successive long blocks; persistent movement indicates that the estimated [posterior moments](../../../../../posterior-moment.md) or tails have not stabilized.
- [Autocorrelation function](../../../../../autocorrelation.md) plots for both parameters after tentative [burn-in](../../../../../burn-in.md). Slow decay reveals strong serial dependence and a small [effective sample size of a Markov chain](../../../../../effective-sample-size-of-a-markov-chain.md), even when $10^6$ iterations have been generated.
- Overlaid [histograms](../../../../../histogram.md) or [kernel density estimation](../../../../../kernel-density-estimation.md) curves from successive retained blocks and from different chains. Their agreement provides evidence of stable marginal [posterior distributions](../../../../../bayesian-posterior.md).
- A [scatter plot](../../../../../scatter-plot.md) of retained $(p,\beta)$ pairs, colored by time block if helpful. Strong dependence or separate clusters can expose slow joint exploration that marginal plots conceal.

**A million iterations and stable-looking plots do not prove convergence.** Agreement across dispersed chains, exploration of all visible modes and adequate [effective sample size of a Markov chain](../../../../../effective-sample-size-of-a-markov-chain.md) provide stronger evidence. Estimate the [Monte Carlo standard error](../../../../../monte-carlo-standard-error.md) using the chain's [autocorrelation](../../../../../autocorrelation.md); the [independent random variables](../../../../../independent-random-variables.md) formula from 3(b)(ii) does not apply directly to these dependent draws.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [C](../../c.md)
3. [3](../../../3.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the simulation and statistical programming course of the University of Oxford](../../../../split.md)
6. [Simulation and statistical programming course of the University of Oxford](../../../../../simulation-and-statistical-programming-course-of-the-university-of-oxford.md)
7. [Year 2 of the mathematics course of the University of Oxford](../../../../../year-2-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
