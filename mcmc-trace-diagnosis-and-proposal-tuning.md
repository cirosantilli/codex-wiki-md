# MCMC trace diagnosis and proposal tuning

↑ **Parent:** [Markov chain Monte Carlo](markov-chain-monte-carlo.md)

A trace of a [Markov chain Monte Carlo](markov-chain-monte-carlo.md) parameter helps distinguish slow movement, long rejection plateaus, and movement between separated regions. Very small random-walk proposals give high acceptance but slow diffusion; very large proposals produce low acceptance and repeated states. Record acceptance rates alongside [trace plots](trace-plot.md) and [effective sample size of a Markov chain](effective-sample-size-of-a-markov-chain.md) before deciding which scale to change. Correlated [posterior](bayesian-posterior.md) directions often benefit from block proposals with a [covariance](covariance.md) fitted during a preliminary tuning run. A trace alone cannot prove convergence or identify the unique cause of poor movement; dispersed chains and stationary summaries provide additional evidence. Freeze tuning before the main sampling phase, or use adaptation satisfying an appropriate ergodicity theorem.

## ↑ Ancestors (7)

1. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/5/a/solution.md)
