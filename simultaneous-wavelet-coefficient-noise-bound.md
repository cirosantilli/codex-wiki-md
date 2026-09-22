# Simultaneous wavelet coefficient noise bound

↑ **Parent:** [Wavelet coefficient thresholding](wavelet-coefficient-thresholding.md)

For coefficient weights $w_{\lambda i}$ and independent mean-zero [sub-Gaussian random variables](sub-gaussian-distribution.md) of parameter $\sigma$, put $q_\lambda^2=\sum_iw_{\lambda i}^2$. Multiplying moment-generating-function bounds shows that the weighted noise has parameter $\sigma q_\lambda$. The exponential Markov inequality, optimized in its parameter, gives tail bound $2\exp(-t^2/(2\sigma^2q_\lambda^2))$. At the displayed thresholds, a [union bound](boole-s-inequality.md) over $N$ coefficients gives simultaneous control with [probability](probability.md) at least $1-\delta$. No coefficient independence is required. Integrated wavelet weights satisfy $q_\lambda\leq n^{-1/2}$. Finite variance alone only supports the weaker Chebyshev choice $\tau_\lambda=\sigma q_\lambda\sqrt{N/\delta}$.

## ↑ Ancestors (10)

1. [Wavelet coefficient thresholding](wavelet-coefficient-thresholding.md)
2. [Wavelet regression estimator](wavelet-regression-estimator.md)
3. [Fixed-design nonparametric regression](fixed-design-nonparametric-regression.md)
4. [Nonparametric regression](nonparametric-regression.md)
5. [Nonparametric statistics](nonparametric-statistics-split.md)
6. [Statistical inference](statistical-inference-split.md)
7. [Probability and statistics](probability-and-statistics-split.md)
8. [Area of mathematics](area-of-mathematics.md)
9. [Mathematics](mathematics-split.md)
10. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/3/solution.md)
- [Wavelet coefficient thresholding](wavelet-coefficient-thresholding.md)
