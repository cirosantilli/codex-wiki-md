# Control variates

↑ **Parent:** [Monte Carlo estimator](monte-carlo-estimator.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Control_variates)

A control variate is a [random variable](random-variable-split.md) with known [expected value](expected-value.md) whose centered value is subtracted from a [Monte Carlo estimator](monte-carlo-estimator.md) to reduce its [variance](variance-split.md). For a mean-zero vector $G$, put $S=\operatorname{Cov}(G)$ and $c=\operatorname{Cov}(G,H)$. When $S$ is invertible, the optimal estimator averages $H-c^TS^{-1}G$ and has variance $(\operatorname{Var}(H)-c^TS^{-1}c)/N$ for $N$ independent draws. Improvement is strict exactly when $c\ne0$.

**Table of contents**

- [Multivariate control variates](multivariate-control-variates.md)
- [Cauchy tail control variate on a bounded interval](cauchy-tail-control-variate-on-a-bounded-interval.md)
- [Posterior score control variate](posterior-score-control-variate.md)

## ↑ Ancestors (6)

1. [Monte Carlo estimator](monte-carlo-estimator.md)
2. [Monte Carlo method](monte-carlo-method.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2001/iii/paper-23/4/c/solution.md)
