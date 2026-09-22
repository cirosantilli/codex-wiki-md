# EM algorithm for zero-inflated Poisson regression

↑ **Parent:** [Zero-inflated Poisson regression](zero-inflated-poisson-regression.md)

The [expectation-maximization algorithm](expectation-maximization-algorithm.md) introduces $Z_i=1$ for a structural zero. Its E-step gives $\tau_i=0$ at positive counts and $\tau_i=\pi_i/[\pi_i+(1-\pi_i)e^{-\mu_i}]$ at zero. The M-step maximizes a logistic [log-likelihood](log-likelihood.md) with fractional responses $\tau_i$ and a Poisson [log-likelihood](log-likelihood.md) with weights $1-\tau_i$. With only a binary predictor, write $n_j$ for group size, $S_j=\sum_{x_i=j}\tau_i$ and $C_j=\sum_{x_i=j}Y_i$; the explicit updates are $\pi_j=S_j/n_j$ and $\mu_j=C_j/(n_j-S_j)$. Log and logit group contrasts recover the regression coefficients, with boundary values interpreted through limits.

## ↑ Ancestors (10)

1. [Zero-inflated Poisson regression](zero-inflated-poisson-regression.md)
2. [Zero-inflated Poisson distribution](zero-inflated-poisson-distribution.md)
3. [Poisson distribution](poisson-distribution.md)
4. [Discrete probability distribution](discrete-probability-distribution-split.md)
5. [Probability distribution](probability-distribution.md)
6. [Probability theory](probability-theory-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/6/a/solution.md)
- [Posterior structural-zero probability](posterior-structural-zero-probability.md)
