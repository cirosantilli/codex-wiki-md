# Gaussian AR1 bridge

↑ **Parent:** [Autoregressive process of order one](autoregressive-process-of-order-one.md)

For a stationary [autoregressive process of order one](autoregressive-process-of-order-one.md) with mean $\mu$, autoregressive coefficient $\phi$ and innovation [variance](variance-split.md) $\sigma^2$, an interior observation conditional on its neighbors has

$$
X_t\mid X_{t-1},X_{t+1}\sim N\left(\mu+\frac{\phi\{X_{t-1}+X_{t+1}-2\mu\}}{1+\phi^2},\frac{\sigma^2}{1+\phi^2}\right).
$$

The [Markov property](markov-property.md) makes the same law valid when all other observations are also conditioned on.

## ↑ Ancestors (8)

1. [Autoregressive process of order one](autoregressive-process-of-order-one.md)
2. [Autoregressive model](autoregressive-model.md)
3. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
4. [Time series](time-series-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/5/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-218/5/d/solution.md)
