# Grouped Poisson likelihood

↑ **Parent:** [Poisson distribution](poisson-distribution.md)

When a [Poisson distribution](poisson-distribution.md) is observed in cells $0,1,\ldots,r-1,\geq r$, the last cell probability is a tail sum, not the probability of exactly $r$. With $p_i(\theta)=e^{-\theta}\theta^i/i!$ and $Q_r(\theta)=1-\sum_{i<r}p_i(\theta)$, telescoping derivatives give $Q_r'=p_{r-1}$. Thus an interior [maximum-likelihood estimate](maximum-likelihood-estimator.md) solves $\sum_{i<r}n_i(i/\theta-1)+n_rp_{r-1}(\theta)/Q_r(\theta)=0$. Substitution of the estimate into these cell probabilities supplies fitted expected counts for a [likelihood-ratio test](likelihood-ratio-test.md). With $r+1$ cells and one regular fitted parameter, the asymptotic [chi-squared distribution](chi-squared-distribution.md) has $r-1$ degrees of freedom. Replacing every grouped tail observation by $r$ changes the data model and generally does not give the grouped maximum likelihood estimate.

## ↑ Ancestors (8)

1. [Poisson distribution](poisson-distribution.md)
2. [Discrete probability distribution](discrete-probability-distribution-split.md)
3. [Probability distribution](probability-distribution-split.md)
4. [Probability theory](probability-theory-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-options-ii-course-of-the-university-of-oxford/2013/o5/d/i/solution.md)
