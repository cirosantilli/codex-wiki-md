# Discrete wavelet transform

↑ **Parent:** [Wavelet](wavelet.md)

A discrete wavelet transform computes multiscale approximation and detail coefficients from sampled data. In the [Haar wavelet](haar-wavelet.md) construction, apply the displayed orthogonal sum/difference transformation to each adjacent pair and repeat on the approximation coefficients. The detail coefficients at each stage and the last approximation coefficient preserve the squared [Euclidean norm](euclidean-norm.md), because the two-by-two transform is orthogonal. For dyadic sample size, multiplying the resulting coefficients by $n^{-1/2}$ gives the normalized coefficients of the [wavelet regression estimator](wavelet-regression-estimator.md) on $[0,1]$. Under independent Gaussian noise, orthogonality preserves the common coefficient noise variance and independence.

## ↑ Ancestors (6)

1. [Wavelet](wavelet.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (1)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/3/solution.md)
