# Concentration of a beta prior near zero

↑ **Parent:** [Beta distribution](beta-distribution.md)

For $\Theta\sim\operatorname{Beta}(1,\beta)$, direct [integration](integral-split.md) of its [probability density function](probability-density-function.md) gives the displayed tail for $0<t<1$. Increasing $\beta$ strictly decreases every such tail [probability](probability.md), and $\Theta$ converges in [probability](probability.md) to zero as $\beta\to\infty$. Its [mean](expected-value-split.md) is $1/(\beta+1)$ and its [variance](variance-split.md) is $\beta/[(\beta+1)^2(\beta+2)]$; both decrease for $\beta>1$. For the [variance](variance-split.md), logarithmic [differentiation](differentiation.md) gives $1/\beta-2/(\beta+1)-1/(\beta+2)<0$ in that range.

After $S$ successes in $N$ conditionally independent [Bernoulli trials](bernoulli-trial.md), [Beta-binomial conjugacy](beta-binomial-conjugacy.md) gives [posterior mean](posterior-mean.md) $(S+1)/(N+\beta+1)$. Its [derivative](derivative.md) with respect to $\beta$ is negative, while the weight $(\beta+1)/(N+\beta+1)$ assigned to the [prior mean](prior-mean.md) is increasing for $N>0$.

## ↑ Ancestors (7)

1. [Beta distribution](beta-distribution.md)
2. [Probability distribution](probability-distribution-split.md)
3. [Probability theory](probability-theory-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-statistics-course-of-the-university-of-oxford/2021/3/a/iii/solution.md)
