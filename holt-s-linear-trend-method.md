<h1 id="holt-s-linear-trend-method">Holt's linear trend method</h1>

↑ **Parent:** [Double exponential smoothing](double-exponential-smoothing.md)

Update the level and slope by $\ell_t=\alpha X_t+(1-\alpha)(\ell_{t-1}+b_{t-1})$ and $b_t=\beta(\ell_t-\ell_{t-1})+(1-\beta)b_{t-1}$, with gains in $(0,1)$. The first update compares the new observation with the previous level extrapolated one step; the second smooths the latest level increment. The displayed forecast extrapolates that local slope. This is a [double exponential smoothing](double-exponential-smoothing.md) method for a nonseasonal trending [time series](time-series-split.md).

## ↑ Ancestors (7)

1. [Double exponential smoothing](double-exponential-smoothing.md)
2. [Exponential smoothing](exponential-smoothing.md)
3. [Time series](time-series-split.md)
4. [Probability and statistics](probability-and-statistics-split.md)
5. [Area of mathematics](area-of-mathematics.md)
6. [Mathematics](mathematics-split.md)
7. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Brown's double exponential smoothing](brown-s-double-exponential-smoothing.md)
- [Double exponential smoothing](double-exponential-smoothing.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/5/solution.md)
