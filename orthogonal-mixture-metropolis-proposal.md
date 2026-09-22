# Orthogonal-mixture Metropolis proposal

↑ **Parent:** [Proposal distribution](proposal-distribution.md)

For a proposal $Y=AX+Z$, with isotropic $Z\sim N(0,I)$ and an independent random [orthogonal matrix](orthogonal-matrix.md) $A$, invariance of the distribution of $A$ under transpose makes the [proposal distribution](proposal-distribution.md) symmetric. Indeed $|y-Ax|=|x-A^Ty|$, and averaging the isotropic Gaussian density over an inversion-invariant law yields $q(x,y)=q(y,x)$. The [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md) therefore accepts with the target density ratio alone.

## ↑ Ancestors (9)

1. [Proposal distribution](proposal-distribution.md)
2. [Metropolis–Hastings algorithm](metropolis-hastings-algorithm.md)
3. [Markov chain Monte Carlo](markov-chain-monte-carlo.md)
4. [Bayesian statistics](bayesian-statistics.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-216/5/solution.md)
