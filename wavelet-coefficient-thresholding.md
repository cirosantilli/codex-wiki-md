# Wavelet coefficient thresholding

↑ **Parent:** [Wavelet regression estimator](wavelet-regression-estimator.md)

Hard thresholding keeps detail coefficients whose magnitude exceeds a prescribed threshold and sets the rest to zero, while retaining the coarse approximation coefficients. [Soft thresholding](soft-thresholding.md) instead uses $\operatorname{sgn}(\widehat b)(|\widehat b|-\tau)_+$. The [simultaneous wavelet coefficient noise bound](simultaneous-wavelet-coefficient-noise-bound.md) motivates thresholds of order $\sigma\sqrt{\log n/n}$ in a normalized Gaussian regression model with at most order $n$ details. This is a nonlinear selection rule: coefficients can be removed individually rather than discarding an entire finest resolution.

**Table of contents**

- [Simultaneous wavelet coefficient noise bound](simultaneous-wavelet-coefficient-noise-bound.md)

## ↑ Ancestors (9)

1. [Wavelet regression estimator](wavelet-regression-estimator.md)
2. [Fixed-design nonparametric regression](fixed-design-nonparametric-regression.md)
3. [Nonparametric regression](nonparametric-regression.md)
4. [Nonparametric statistics](nonparametric-statistics-split.md)
5. [Statistical inference](statistical-inference-split.md)
6. [Probability and statistics](probability-and-statistics-split.md)
7. [Area of mathematics](area-of-mathematics.md)
8. [Mathematics](mathematics-split.md)
9. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/3/solution.md)
