# Haar scaling function

↑ **Parent:** [Haar wavelet](haar-wavelet.md)

At level $J$, a [Haar scaling function](haar-scaling-function.md) is the normalized [indicator function](indicator-function.md) $\phi_{J,k}=2^{J/2}\mathbf1_{I_{J,k}}$ of the [dyadic interval](dyadic-interval.md) $I_{J,k}=[k2^{-J},(k+1)2^{-J})$. Its [L2 norm](l2-norm.md) is one because its squared height is $2^J$ and its support length is $2^{-J}$.

For a real [square-integrable function](square-integrable-function.md) $f$, its coefficient is

$$
\langle f,\phi_{J,k}\rangle
=2^{J/2}\int_{I_{J,k}}f(x)\,dx
=2^{-J/2}\overline f_{I_{J,k}}.
$$

Multiplying the coefficient by the [Haar scaling function](haar-scaling-function.md) restores the [cell average](average-value-of-a-function.md) on that interval. The disjoint [supports](support.md) make the functions at one level an [orthonormal basis](orthonormal-basis.md) of the cellwise-constant subspace. This normalization is also what turns coefficient [variances](variance-split.md) in the [Gaussian white noise model](gaussian-white-noise-model.md) into $1/n$ and cellwise variances into $2^J/n$ in the [Haar projection estimator in Gaussian white noise](haar-projection-estimator-in-gaussian-white-noise.md).

## ↑ Ancestors (8)

1. [Haar wavelet](haar-wavelet.md)
2. [Orthonormal wavelet](orthonormal-wavelet.md)
3. [Wavelet](wavelet.md)
4. [Fourier analysis](fourier-analysis-split.md)
5. [Analysis](analysis-split.md)
6. [Area of mathematics](area-of-mathematics.md)
7. [Mathematics](mathematics-split.md)
8. [Codex Wiki](split.md)

## ← Incoming links (11)

- [Dyadic partition](dyadic-partition.md)
- [Haar density estimator](haar-density-estimator.md)
- [Haar projection](haar-projection.md)
- [Haar projection estimator in Gaussian white noise](haar-projection-estimator-in-gaussian-white-noise.md)
- [Haar refinement identity](haar-refinement-identity.md)
- [Haar scaling function](haar-scaling-function.md)
- [Haar wavelet](haar-wavelet.md)
- [Orthonormal wavelet](orthonormal-wavelet.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2009/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2013/iii/paper-33/3/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2015/iii/paper-36/2/solution.md)
