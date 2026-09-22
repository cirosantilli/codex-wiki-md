# Filtered backprojection

↑ **Parent:** [Radon transform](radon-transform.md)

The [Radon transform](radon-transform.md) records line integrals of a planar density. Apply the transverse [Hilbert transform](hilbert-transform.md) and a derivative to each projection, then average the filtered values over all lines through the reconstruction point. With $Hh(\rho)=\pi^{-1}\operatorname{PV}\int h(r)/(\rho-r)dr$, the filter has [Fourier multiplier](fourier-multiplier.md) $|\kappa|$. The [Fourier inversion theorem](fourier-inversion-theorem.md), or the jump of the [complexified transport Cauchy kernel](complexified-transport-cauchy-kernel.md), proves the displayed formula. The factor is $1/(2\pi)$ when directions are integrated over a half-circle. The growing [Fourier multiplier](fourier-multiplier.md) explains amplification of measurement noise and the need for [regularization of an inverse problem](regularization-of-an-inverse-problem.md).

## ↑ Ancestors (6)

1. [Radon transform](radon-transform.md)
2. [Integral transform](integral-transform.md)
3. [Analysis](analysis-split.md)
4. [Area of mathematics](area-of-mathematics.md)
5. [Mathematics](mathematics-split.md)
6. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Computed tomography](computed-tomography.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-67/2/d/solution.md)
- [Solution](past-exam-of-the-mathematics-course-of-the-university-of-cambridge/2005/iii/paper-67/2/e/solution.md)
