# Stationary Gaussian AR1 likelihood

↑ **Parent:** [Autoregressive process of order one](autoregressive-process-of-order-one.md)

For $|\phi|<1$, independent $N(0,\sigma^2)$ innovations and stationary initial variance $\sigma^2/(1-\phi^2)$, the full [likelihood function](likelihood-function.md) is

$$
L=(2\pi\sigma^2)^{-n/2}\sqrt{1-\phi^2}\exp\left[-\frac{(1-\phi^2)(x_1-\mu)^2+\sum_{t=2}^n\{(x_t-\mu)-\phi(x_{t-1}-\mu)\}^2}{2\sigma^2}\right].
$$

Conditioning on $X_1$ gives a different likelihood.

**Table of contents**

- [Conditional and stationary AR1 likelihood estimators](conditional-and-stationary-ar1-likelihood-estimators.md)

## ↑ Ancestors (8)

1. [Autoregressive process of order one](autoregressive-process-of-order-one.md)
2. [Autoregressive model](autoregressive-model.md)
3. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
4. [Time series](time-series-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/5/b/solution.md)
