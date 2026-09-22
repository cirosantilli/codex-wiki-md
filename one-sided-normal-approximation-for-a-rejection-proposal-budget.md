# One-sided normal approximation for a rejection proposal budget

↑ **Parent:** [Binomial count and iid values in fixed-budget rejection sampling](binomial-count-and-iid-values-in-fixed-budget-rejection-sampling.md)

For [rejection sampling](rejection-sampling.md) with acceptance [probability](probability.md) $1/M$, $M>1$, the accepted count in $n$ trials has [binomial distribution](binomial-distribution.md), mean $n/M$ and [variance](variance-split.md) $n(M-1)/M^2$. To obtain at least $N$ acceptances with approximate [probability](probability.md) $1-\delta$, use the [standard normal distribution](standard-normal-distribution.md) [quantile](quantile-function.md) $z=\Phi^{-1}(1-\delta)$. The [central limit theorem](central-limit-theorem.md) without continuity correction gives $n-MN\geq z\sqrt{n(M-1)}$. Solving this [quadratic inequality](quadratic-inequality.md) in $\sqrt n$ gives the displayed threshold, rounded upward. It exceeds the average stopping cost $MN$ because it allows for fluctuations in the accepted count. For $M=1$, the count is deterministic and $n=N$ exactly. Exact coverage uses the [binomial distribution](binomial-distribution.md) tail rather than the approximation.

## ↑ Ancestors (7)

1. [Binomial count and iid values in fixed-budget rejection sampling](binomial-count-and-iid-values-in-fixed-budget-rejection-sampling.md)
2. [Rejection sampling](rejection-sampling.md)
3. [Monte Carlo method](monte-carlo-method-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-simulation-and-statistical-programming-course-of-the-university-of-oxford/2023/1/b/iii/solution.md)
