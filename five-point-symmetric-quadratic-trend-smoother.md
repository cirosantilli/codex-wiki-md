# Five-point symmetric quadratic trend smoother

↑ **Parent:** [Time series](time-series-split.md)

For observations $X_t=T_t+\varepsilon_t$ with a quadratic trend and uncorrelated equal-variance errors, a symmetric five-point [linear filter of a stationary time series](linear-filter-of-a-stationary-time-series.md) has weights $(a,b,c,b,a)$. Reproducing every quadratic requires $2a+2b+c=1$ and $8a+2b=0$. Substitution gives $b=-4a$, $c=1+6a$ and error [variance](variance-split.md) $\sigma^2(70a^2+12a+1)$. Its unique minimum occurs at $a=-3/35$, producing the displayed weights and [variance](variance-split.md) $17\sigma^2/35$. Negative weights are allowed: this is a linear weighted smoother, not a convex average. Applying a linear filter to a deterministic trend plus stationary errors does not assert that the complete observation process is stationary.

## ↑ Ancestors (5)

1. [Time series](time-series-split.md)
2. [Probability and statistics](probability-and-statistics-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2002/iii/paper-40/5/solution.md)
- [Three-point quadratic reproduction forces the identity filter](three-point-quadratic-reproduction-forces-the-identity-filter.md)
