# Semidiscrete Fourier transform

↑ **Parent:** [Fourier analysis](fourier-analysis-split.md)

For a sequence indexed by the [integers](integer-split.md), its semidiscrete Fourier transform is the displayed [Fourier series](fourier-series-split.md) in $\theta\in[-\pi,\pi]$. For square-summable data the series is interpreted in the [L2 norm](l2-norm.md). Its inversion and [Parseval identity](parseval-identity.md) are

$$
W_j=\frac1{2\pi}\int_{-\pi}^{\pi}\widehat W(\theta)e^{ij\theta}d\theta,\qquad
h\sum_{j\in\mathbb Z}|W_j|^2=\frac h{2\pi}\int_{-\pi}^{\pi}|\widehat W(\theta)|^2d\theta.
$$

The physical-frequency convention uses $\theta=kh$ and $\widetilde W(k)=h\widehat W(kh)$ on $[-\pi/h,\pi/h]$. This is distinct from the [discrete Fourier transform](discrete-fourier-transform-split.md) of a finite vector. Translation-invariant [finite difference operators](finite-difference-operator.md) become [Fourier multipliers](fourier-multiplier.md), making [Fourier stability analysis](fourier-stability-analysis.md) possible.

**Table of contents**

- [Fourier stability threshold for a mixed-width heat scheme](fourier-stability-threshold-for-a-mixed-width-heat-scheme.md)

## ↑ Ancestors (5)

1. [Fourier analysis](fourier-analysis-split.md)
2. [Analysis](analysis-split.md)
3. [Area of mathematics](area-of-mathematics.md)
4. [Mathematics](mathematics-split.md)
5. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Solution](past-exam-of-the-numerical-solution-of-differential-equations-course-of-the-university-of-oxford/2010/a/2/a/solution.md)
- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/3/b/solution.md)
- [Solution](past-exam-of-the-numerical-solutions-of-partial-differential-equations-course-of-the-university-of-oxford/2023/3/d/solution.md)
