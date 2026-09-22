# Zero-event binomial upper confidence bound

↑ **Parent:** [Binomial distribution](binomial-distribution.md)

If $X\sim\operatorname{Bin}(n,p)$ and $X=0$ is observed, the [maximum-likelihood estimate](maximum-likelihood-estimator.md) of $p$ is zero. A one-sided $1-\alpha$ upper [confidence bound](confidence-bound.md) solves $P_{p_U}(X=0)=(1-p_U)^n=\alpha$, so $p_U=1-\alpha^{1/n}$. For large $n$, $p_U\simeq-\log(\alpha)/n$, giving approximately $3/n$ at 95% confidence. This describes uncertainty after no observed events, rather than proving that the underlying [probability](probability.md) is zero. It assumes independent observations with a common event probability; [clustered data](clustered-data.md) require a different uncertainty calculation.

## ↑ Ancestors (8)

1. [Binomial distribution](binomial-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-37/3/iv/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-34/1/b/solution.md)
