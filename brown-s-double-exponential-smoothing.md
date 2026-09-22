<h1 id="brown-s-double-exponential-smoothing">Brown's double exponential smoothing</h1>

↑ **Parent:** [Double exponential smoothing](double-exponential-smoothing.md)

For $0<\alpha<1$, set $s_t^{(1)}=\alpha X_t+(1-\alpha)s_{t-1}^{(1)}$ and $s_t^{(2)}=\alpha s_t^{(1)}+(1-\alpha)s_{t-1}^{(2)}$. Use the displayed corrected level and slope, then forecast $a_t+hb_t$. For an exact linear trend after initialization transients, the first and second smooths have lags $(1-\alpha)/\alpha$ and twice that lag; their difference recovers the slope and the corrected level removes the lag. This is distinct from [Holt's linear trend method](holt-s-linear-trend-method.md).

## ↑ Ancestors (7)

1. [Double exponential smoothing](double-exponential-smoothing.md)
2. [Exponential smoothing](exponential-smoothing.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Double exponential smoothing](double-exponential-smoothing.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/5/solution.md)
