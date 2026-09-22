# Seasonal differencing does not remove periodic variance

↑ **Parent:** [Seasonal difference operator](seasonal-difference-operator.md)

If $X_t=c_t\varepsilon_t$ with a deterministic periodic scale $c_t=c_{t-S}$ and [strong white noise](strong-white-noise.md) of variance $\sigma^2$, then $\Delta_SX_t=c_t(\varepsilon_t-\varepsilon_{t-S})$. Its variance is $2\sigma^2c_t^2$, still seasonal when $c_t^2$ varies. A periodic scale model or variance standardization is more appropriate than blindly applying [differencing](differencing.md).

## ↑ Ancestors (7)

1. [Seasonal difference operator](seasonal-difference-operator.md)
2. [Differencing](differencing.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2016/iii/paper-208/3/3/solution.md)
- [Seasonality](seasonality.md)
