<h1 id="finite-sample-innovations-of-an-ma-1-process">Finite-sample innovations of an MA(1) process</h1>

↑ **Parent:** [Best linear prediction from a finite past](best-linear-prediction-from-a-finite-past.md)

Starting at time one, the orthogonal residuals satisfy $U_t=X_t-\lambda_tU_{t-1}$, with $\lambda_t=\gamma_1/\varphi_{t-1}$ and $\varphi_t=\gamma_0-\gamma_1\lambda_t$. Earlier innovation directions have zero [covariance](covariance.md) with the new observation. Explicitly, with $S_m=\sum_{j=0}^m\theta^{2j}$, $\varphi_t=\sigma^2S_t/S_{t-1}$ and $\lambda_t=\theta S_{t-2}/S_{t-1}$ for $t\ge2$. These formulas follow by induction from $S_t=(1+\theta^2)S_{t-1}-\theta^2S_{t-2}$, with $S_0=1$ and $S_1=1+\theta^2$. This includes $\theta=\pm1$, where $\varphi_t=\sigma^2(t+1)/t$.

**Table of contents**

- [Limiting MA(1) innovations coefficient](limiting-ma-1-innovations-coefficient.md)

## ↑ Ancestors (6)

1. [Best linear prediction from a finite past](best-linear-prediction-from-a-finite-past.md)
2. [Time series](time-series-split.md)
3. [Probability and statistics](probability-and-statistics-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Autocovariance of an MA(1) process](autocovariance-of-an-ma-1-process.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-38/2/solution.md)
