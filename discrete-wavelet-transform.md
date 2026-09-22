# Discrete wavelet transform

↑ **Parent:** [Wavelet](wavelet.md)

A discrete wavelet transform computes multiscale approximation and detail coefficients from sampled data. For the [Haar wavelet](haar-wavelet.md), replace each adjacent pair $(u,v)$ by

$$
a=\frac{u+v}{\sqrt2},\qquad d=\frac{u-v}{\sqrt2}.
$$

The approximation coefficient $a$ is $\sqrt2$ times the pair's [arithmetic mean](arithmetic-mean.md); it is not the ordinary mean. The detail coefficient $d$ records their signed contrast. Repeat on the approximation coefficients until only one remains, keeping every detail coefficient.

For a worked example, start with the vector $(2,4,6,8)$. The first pass gives approximation coefficients $(3\sqrt2,7\sqrt2)$ and detail coefficients $(-\sqrt2,-\sqrt2)$. Transforming the remaining pair gives the coarse coefficient $10$ and the half-to-half detail $-4$. In the order coarse value, coarse detail, then fine details, the transform is

$$
\boxed{(2,4,6,8)\longmapsto(10,-4,-\sqrt2,-\sqrt2).}
$$

This is an [orthogonal matrix](orthogonal-matrix.md) transformation. Each pair preserves $u^2+v^2=a^2+d^2$, so the full transform preserves the squared [Euclidean norm](euclidean-norm.md):

$$
2^2+4^2+6^2+8^2=120=10^2+(-4)^2+(-\sqrt2)^2+(-\sqrt2)^2.
$$

The [inverse function](inverse-function.md) for each pair is $u=(a+d)/\sqrt2$, $v=(a-d)/\sqrt2$. Reversing the passes therefore recovers every original value. This squared-norm bookkeeping is often called signal energy; it need not represent physical [energy](energy-split.md). [MathWorks: Haar transforms, approximation/detail coefficients and squared-norm conservation](https://www.mathworks.com/help/wavelet/ug/haar-transforms-for-time-series-data-and-images.html)

Continuous and discrete normalizations differ. If $n=2^J$ data values are interpreted as the heights of a [step function](step-function.md) on $n$ equal cells of $[0,1]$, its normalized [L2 inner product](l2-inner-product.md) coefficients are the discrete coefficients divided by $\sqrt n$. For our four values they are $(5,-2,-1/\sqrt2,-1/\sqrt2)$, as the [Haar projection](haar-projection.md) example shows. The same normalization is used by the [wavelet regression estimator](wavelet-regression-estimator.md) on $[0,1]$.

Under [independent](independent-random-variables.md) [Gaussian noise](gaussian-noise.md) with a common [variance](variance-split.md), [orthogonality](orthogonal-vectors.md) preserves that coefficient noise [variance](variance-split.md) and independence. It does not make every arbitrary correlated [signal](signal.md) independent: this statistical conclusion uses the Gaussian model and its equal-variance independent inputs.

## ↑ Ancestors (6)

1. [Wavelet](wavelet.md)
2. [Fourier analysis](fourier-analysis-split.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2010/iii/paper-31/3/solution.md)
- [Wavelet](wavelet.md)
