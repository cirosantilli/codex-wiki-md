# Zero-inflated Poisson regression

↑ **Parent:** [Zero-inflated Poisson distribution](zero-inflated-poisson-distribution.md)

A zero-inflated Poisson regression specifies a structural-zero probability $\pi$ and a susceptible-component [Poisson distribution](poisson-distribution.md) mean $\mu$. In this parametrization,

$$
P(Y=0)=\pi+(1-\pi)e^{-\mu},\qquad P(Y=y)=(1-\pi)e^{-\mu}\mu^y/y!\quad(y>0).
$$

The mean is $(1-\pi)\mu$. Logistic predictors for $\pi$ and logarithmic predictors for $\mu$ allow covariates to affect component membership and count intensity differently. A susceptible individual can still generate a zero count; susceptibility is not equivalent to an observed positive response.

**Table of contents**

- [Posterior structural-zero probability](posterior-structural-zero-probability.md)
- [Component and marginal effects in zero-inflated regression](component-and-marginal-effects-in-zero-inflated-regression.md)
- [EM algorithm for zero-inflated Poisson regression](em-algorithm-for-zero-inflated-poisson-regression.md)

## ↑ Ancestors (9)

1. [Zero-inflated Poisson distribution](zero-inflated-poisson-distribution.md)
2. [Poisson distribution](poisson-distribution.md)
3. [Discrete probability distribution](discrete-probability-distribution-split.md)
4. [Probability distribution](probability-distribution.md)
5. [Probability theory](probability-theory-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (4)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/6/b/i/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2014/iii/paper-33/6/b/ii/solution.md)
- [Posterior structural-zero probability](posterior-structural-zero-probability.md)
