# Fibonacci-coefficient autoregression

↑ **Parent:** [Autoregressive model](autoregressive-model.md)

For $X_t=\alpha X_{t-1}+\alpha^2X_{t-2}+\varepsilon_t$, let $\varphi=(1+\sqrt5)/2$. The autoregressive [polynomial](polynomial-split.md) factors as $(1-\alpha\varphi z)(1+\alpha z/\varphi)$. Its roots lie outside the closed [unit disk](unit-disk.md) exactly when $|\alpha|<1/\varphi$. In that causal region,

$$
X_t=\sum_{j\geq0}F_{j+1}\alpha^j\varepsilon_{t-j},\qquad
F_{j+1}=\frac{\varphi^{j+1}-(-1/\varphi)^{j+1}}{\sqrt5}.
$$

The coefficients follow from $\psi_0=1,\psi_1=\alpha$ and $\psi_j=\alpha\psi_{j-1}+\alpha^2\psi_{j-2}$. They are absolutely summable in the stated region. Causality makes future [white noise](white-noise.md) orthogonal to the observation past, giving forecasts $\alpha X_T+\alpha^2X_{T-1}$ and $2\alpha^2X_T+\alpha^3X_{T-1}$ at horizons one and two.

## ↑ Ancestors (7)

1. [Autoregressive model](autoregressive-model.md)
2. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-47/2/solution.md)
