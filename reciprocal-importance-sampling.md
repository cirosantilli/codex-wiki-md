# Reciprocal importance sampling

↑ **Parent:** [Importance sampling](importance-sampling.md)

Let $r$ be an unnormalized density, $Z=\int r$ with $0<Z<\infty$, and $\pi=r/Z$. Given independent draws $\theta_t\sim\pi$ and an evaluable normalized density $q$ supported where $r>0$, reciprocal importance sampling estimates $Z^{-1}$ by $T^{-1}\sum_tq(\theta_t)/r(\theta_t)$. Its [expectation](expected-value-split.md) is $Z^{-1}\int q=Z^{-1}$ and its [variance](variance-split.md) is $(TZ^2)^{-1}(\int q^2/\pi-1)$. Broad tails of $q$ relative to $\pi$ can make this infinite; reversing the [importance sampling](importance-sampling.md) ratio reverses the dangerous tail mismatch. Taking the reciprocal of the estimate is generally biased for $Z$.

## ↑ Ancestors (6)

1. [Importance sampling](importance-sampling.md)
2. [Monte Carlo method](monte-carlo-method-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-advanced-topics-in-statistical-machine-learning-course-of-the-university-of-oxford/2025/1/b/iii/solution.md)
