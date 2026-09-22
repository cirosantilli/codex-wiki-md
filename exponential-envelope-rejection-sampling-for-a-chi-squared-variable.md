# Exponential-envelope rejection sampling for a chi-squared variable

↑ **Parent:** [Rejection sampling](rejection-sampling.md)

Write $a=\nu/2$. Against an [exponential distribution](exponential-distribution.md) proposal of mean $\nu$, the [chi-squared distribution](chi-squared-distribution.md) density has envelope constant $M=a^ae^{1-a}/\Gamma(a)$. The density ratio divided by $M$ is $\exp((a-1)(\log(y/\nu)-y/\nu+1))$. Thus generate $Y=-\nu\log U$ and accept when $\log V\leq(a-1)(\log(Y/\nu)-Y/\nu+1)$ for independent [uniform distributions](continuous-uniform-distribution.md). The inequality $\log t\leq t-1$ validates the acceptance probability. The accepted [probability density function](probability-density-function.md) is the target because [rejection sampling](rejection-sampling.md) weights the proposal by its target-to-envelope ratio.

## ↑ Ancestors (6)

1. [Rejection sampling](rejection-sampling.md)
2. [Monte Carlo method](monte-carlo-method.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2008/iii/paper-47/3/b/ii/solution.md)
