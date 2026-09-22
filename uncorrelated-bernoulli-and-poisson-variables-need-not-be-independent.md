# Uncorrelated Bernoulli and Poisson variables need not be independent

↑ **Parent:** [Uncorrelated random variables](uncorrelated-random-variables.md)

Here is an explicit joint distribution, for $0<p<0.8$: assign mass $(1+p)e^{-p}-p$ at $(0,0)$, mass $p(1-e^{-p})$ at $(1,0)$, mass $pe^{-p}$ at $(1,1)$, and mass $e^{-p}p^k/k!$ at $(0,k)$ for $k\geq2$; all other masses are zero. These are nonnegative: the first is decreasing in $p$, and at $p=0.8$ it is still positive. Summing over rows and columns gives a [Bernoulli distribution](bernoulli-distribution.md) with mean $p$ and a [Poisson distribution](poisson-distribution.md) with mean $p$, so the joint mass sums to one.

Only $(1,1)$ contributes to the mixed first [moment](moment.md), giving $\mathbb E[XY]=pe^{-p}$ and the [covariance](covariance.md) above. The strictly decreasing [function](function-split.md) $e^{-p}-p$ has a unique zero in $(0,0.8)$, approximately $0.567143$. At that parameter the variables are uncorrelated. They are nevertheless dependent, because $\mathbb P(X=1\mid Y=1)=1$ whereas $\mathbb P(X=1)=p<1$. The [Bernoulli independence from zero covariance](bernoulli-independence-from-zero-covariance.md) result requires both variables to be Bernoulli and does not apply here.

## ↑ Ancestors (9)

1. [Uncorrelated random variables](uncorrelated-random-variables.md)
2. [Covariance](covariance.md)
3. [Variance](variance-split.md)
4. [Expected value](expected-value-split.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-year-1-of-the-computer-science-course-of-the-university-of-oxford/2022/discrete-mathematics-continuous-mathematics-and-probability-resit/7/b/iv/solution.md)
