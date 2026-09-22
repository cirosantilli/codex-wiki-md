# Orthonormal wavelet

↑ **Parent:** [Wavelet](wavelet.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Orthonormal_wavelet)

An orthonormal wavelet $\psi$ generates an [orthonormal basis](orthonormal-basis.md) of $L^2(\mathbb R)$ through

$$
\psi_{j,k}(x)=2^{j/2}\psi(2^jx-k),\qquad j,k\in\mathbb Z.
$$

The factor $2^{j/2}$ compensates for the shrinking [support of a function](support.md), keeping the [L2 norm](l2-norm.md) equal to one. [Orthogonality](orthogonal-vectors.md) makes different coefficients separate squared-norm contributions, and completeness allows the [wavelet series](wavelet-series.md) to recover any [square-integrable function](square-integrable-function.md) in the [L2 norm](l2-norm.md).

For the [Haar wavelet](haar-wavelet.md), wavelets at one scale have disjoint [supports](support.md). At different scales their [dyadic intervals](dyadic-interval.md) are either disjoint or nested. On the support of the finer wavelet, the coarser one is constant, while the finer one has zero [integral](integral-split.md), so their [L2 inner product](l2-inner-product.md) is zero. Together with the unit [L2 norm](l2-norm.md), this explains [orthonormality](orthonormal-set.md). On the bounded [interval](interval-mathematics.md) $[0,1]$, add the constant [Haar scaling function](haar-scaling-function.md) and use $j\geq0$, $0\leq k<2^j$; the constant function is not an $L^2(\mathbb R)$ basis element on the whole line.

**Table of contents**

- [Daubechies wavelet](daubechies-wavelet.md)
- [Haar wavelet](haar-wavelet.md)
  - [Uniform hard-threshold convergence of normalized Haar expansions](uniform-hard-threshold-convergence-of-normalized-haar-expansions.md)
    - [Geometric bound for omitted Haar details](geometric-bound-for-omitted-haar-details.md)
  - [Haar refinement identity](haar-refinement-identity.md)
  - [Haar projection](haar-projection.md)
    - [Haar projection error for a Lipschitz function](haar-projection-error-for-a-lipschitz-function.md)
    - [Haar approximation error for a function of bounded variation](haar-approximation-error-for-a-function-of-bounded-variation.md)
    - [Haar projection estimator in Gaussian white noise](haar-projection-estimator-in-gaussian-white-noise.md)
      - [Supremum norm risk of a Haar projection estimator](supremum-norm-risk-of-a-haar-projection-estimator.md)
  - [Haar scaling function](haar-scaling-function.md)

## ↑ Ancestors (6)

1. [Wavelet](wavelet.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (16)

- [Best N-term wavelet approximation of piecewise Hölder functions](best-n-term-wavelet-approximation-of-piecewise-holder-functions.md)
- [Daubechies wavelet](daubechies-wavelet.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-62/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2012/iii/paper-70/6/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-69/2/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2017/iii/paper-340/1/b/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/1/a/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/1/c/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2018/iii/paper-340/6/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2025/iii/paper-318/5/a/solution.md)
- [Wavelet](wavelet.md)
- [Wavelet completion of a multiresolution filter](wavelet-completion-of-a-multiresolution-filter.md)
- [Wavelet polynomial annihilation](wavelet-polynomial-annihilation.md)
- [Wavelet series](wavelet-series.md)
