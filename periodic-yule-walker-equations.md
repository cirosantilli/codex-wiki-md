# Periodic Yule-Walker equations

↑ **Parent:** [Periodic autoregressive model of order one](periodic-autoregressive-model-of-order-one.md)

For unit-variance innovations, orthogonality to the past gives

$$
\gamma_\nu(h)=\phi_\nu\gamma_{\nu-1}(h-1)\quad(h\geq1),\qquad V_\nu=\phi_\nu^2V_{\nu-1}+\sigma_\nu^2.
$$

Consequently $\phi_\nu=\gamma_\nu(1)/V_{\nu-1}$ and $\sigma_\nu^2=V_\nu-\gamma_\nu(1)^2/V_{\nu-1}$. Replacing [autocovariance](autocovariance.md) by matched sample estimates yields seasonal regression estimators. The unit innovation variance is necessary to identify the noise scale separately.

## ↑ Ancestors (8)

1. [Periodic autoregressive model of order one](periodic-autoregressive-model-of-order-one.md)
2. [Autoregressive model](autoregressive-model.md)
3. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
4. [Time series](time-series-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/3/3/4/solution.md)
