# Bayes estimator under weighted absolute loss

↑ **Parent:** [Bayes estimator](bayes-estimator.md)

Under loss $w(\theta)|\theta-a|$, assume $0<\mathbb E[w(\theta)\mid x]<\infty$. The [posterior expected loss](posterior-expected-loss.md) is a positive constant times ordinary [absolute-error loss](absolute-error-loss.md) under the probability density proportional to $w(\theta)\pi(\theta\mid x)$. Its minimizers are the [medians](median.md) of that weighted posterior: slopes of the loss change sign where the weighted probability below $a$ crosses one half. In particular, relative absolute loss has $w(\theta)=1/\theta$ for positive parameters. For a [Gamma distribution](gamma-distribution.md) posterior of shape two and rate $b$, the weighted posterior is an [exponential distribution](exponential-distribution.md) of rate $b$, so the estimate is $(\log2)/b$.

## ↑ Ancestors (7)

1. [Bayes estimator](bayes-estimator.md)
2. [Bayesian statistics](bayesian-statistics.md)
3. [Statistical inference](statistical-inference-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2004/ib/paper-4/19h/ii/solution.md)
