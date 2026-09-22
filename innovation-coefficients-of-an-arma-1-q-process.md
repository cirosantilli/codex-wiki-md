<h1 id="innovation-coefficients-of-an-arma-1-q-process">Innovation coefficients of an ARMA(1,q) process</h1>

↑ **Parent:** [Autoregressive moving-average model](autoregressive-moving-average-model.md)

With $\theta_0=1$ and $|\phi|<1$, expand the transfer function $\Theta(z)/(1-\phi z)$ by its geometric series. Its coefficient of $z^j$ is the displayed expression; after $j=q$ the coefficients follow a geometric tail. Causality gives $\operatorname{Cov}(\epsilon_{t-i},X_{t-k})=\sigma^2c_{i-k}$ for $i\ge k$, and zero otherwise. Hence $\gamma_k-\phi\gamma_{k-1}=\sigma^2\sum_{i=k}^q\theta_i c_{i-k}$ for $0\le k\le q$, with $\gamma_{-1}=\gamma_1$ in the zero-lag equation.

## ↑ Ancestors (6)

1. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-40/1/solution.md)
