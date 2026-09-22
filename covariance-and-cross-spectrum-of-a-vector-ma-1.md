<h1 id="covariance-and-cross-spectrum-of-a-vector-ma-1">Covariance and cross-spectrum of a vector MA(1)</h1>

↑ **Parent:** [Multivariate moving-average model](multivariate-moving-average-model.md)

For $Z_t=W_t+\Theta W_{t-1}$ and vector [white noise](white-noise.md) of [covariance matrix](covariance-matrix.md) $D$, the only nonzero covariance lags are $\Gamma(0)=D+\Theta D\Theta^T$, $\Gamma(1)=D\Theta^T$ and $\Gamma(-1)=\Theta D$. This follows by retaining only matching noise times in $\mathbb E[Z_tZ_{t+h}^T]$. Its spectral matrix, with this lag convention, is $(I+\Theta e^{i\lambda})D(I+\Theta^Te^{-i\lambda})/(2\pi)$. In two dimensions, with $D=\operatorname{diag}(a,b)$, its cross-spectrum is $[a\theta_{11}\theta_{21}+b\theta_{12}\theta_{22}+a\theta_{21}e^{-i\lambda}+b\theta_{12}e^{i\lambda}]/(2\pi)$.

## ↑ Ancestors (8)

1. [Multivariate moving-average model](multivariate-moving-average-model.md)
2. [Moving-average model](moving-average-model.md)
3. [Autoregressive moving-average model](autoregressive-moving-average-model.md)
4. [Time series](time-series-split.md)
5. [Probability and statistics](probability-and-statistics-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2007/iii/paper-48/2/solution.md)
