# Normal rejection sampling with an exponential envelope

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

For the [half-normal distribution](half-normal-distribution.md), the density ratio to $\operatorname{Exp}(\lambda)$ is maximized at $y=\lambda$. Completing the square gives the envelope constant above and acceptance [probability](probability.md) $e^{-(y-\lambda)^2/2}$. Its logarithmic derivative is $\lambda-1/\lambda$, so the optimal rate is $\lambda=1$. Give an accepted nonnegative value an independent fair sign to obtain the [standard normal distribution](standard-normal-distribution.md). The expected number of proposals is $M$, while the [probability](probability.md) of rejecting one proposal is $1-1/M$; these are different quantities.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-33/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-33/3/solution.md)
