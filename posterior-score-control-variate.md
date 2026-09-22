# Posterior score control variate

↑ **Parent:** [Control variates](control-variates.md)

If a smooth [posterior density](posterior-density.md) has vanishing boundary terms, its [log-posterior](log-posterior.md) gradient satisfies $\mathbb E[g]=0$ and

$$
\mathbb E[g(\beta)h(\beta)]=-\mathbb E[\nabla h(\beta)].
$$

This is a posterior integration-by-parts identity; it concerns differentiation in the random parameter, distinct from the usual [mean-zero score identity](mean-zero-score-identity.md) for sampling distributions. It makes $g$ a vector [control variate](control-variates.md). Finite moments and known coefficients preserve unbiasedness of the [Monte Carlo estimator](monte-carlo-estimator.md).

## ↑ Ancestors (7)

1. [Control variates](control-variates.md)
2. [Monte Carlo estimator](monte-carlo-estimator.md)
3. [Monte Carlo method](monte-carlo-method.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Log-posterior](log-posterior.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/6/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/6/c/solution.md)
- [Probit posterior score](probit-posterior-score.md)
