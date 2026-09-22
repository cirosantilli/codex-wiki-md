# Empty component under an improper prior

↑ **Parent:** [Posterior propriety](posterior-propriety.md)

If a model configuration leaves a parameter absent from its [likelihood function](likelihood-function.md), giving that parameter an independent flat [improper prior](improper-prior.md) makes the [posterior distribution](bayesian-posterior.md) normalization infinite whenever the configuration has positive [prior distribution](prior-probability.md) mass. Integrate first over that parameter: a positive constant [likelihood function](likelihood-function.md) factor is repeated over all of $\mathbb R$. This occurs for the second segment mean of a [Gaussian](normal-distribution.md) [change-point detection](change-point-detection.md) model when the proposed split is after the final observation. There is no [posterior distribution](bayesian-posterior.md) or valid [Gibbs sampler](gibbs-sampler.md) for that joint kernel. A proper [prior distribution](prior-probability.md) on the unused parameter is necessary if the no-change configuration is retained.

## ↑ Ancestors (9)

1. [Posterior propriety](posterior-propriety.md)
2. [Improper prior](improper-prior.md)
3. [Bayesian posterior](bayesian-posterior.md)
4. [Bayesian statistics](bayesian-statistics.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/5/solution.md)
