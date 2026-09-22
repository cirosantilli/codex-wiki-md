<h1 id="3/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

Write $z=x+iy$ and $\overline z=x-iy$. A convenient [spectral parameter for a linear boundary value problem](../../../../../../spectral-parameter-for-a-linear-boundary-value-problem.md) is any $\lambda\in\mathbb C\setminus\{0\}$. Define the [modified Helmholtz adjoint plane wave](../../../../../../modified-helmholtz-adjoint-plane-wave.md)

$$
\boxed{v_\lambda(z,\overline z)=\exp\!\left[\frac{ik}{2}\left(\lambda z-\frac{\overline z}{\lambda}\right)\right]=e^{A(\lambda)x+B(\lambda)y},}
$$

where

$$
A(\lambda)=\frac{ik}{2}(\lambda-\lambda^{-1}),\qquad B(\lambda)=-\frac k2(\lambda+\lambda^{-1}).
$$

Indeed $A^2+B^2=k^2$, so $(\Delta-k^2)v_\lambda=0$. Equivalently, $4\partial_z\partial_{\overline z}v_\lambda=k^2v_\lambda$. The exclusion of zero is only the coordinate singularity of this spectral parametrization; it still supplies a whole complex one-parameter family. The conjugate companion is

$$
\widetilde v_\lambda=\exp\!\left[-\frac{ik}{2}\left(\lambda\overline z-\frac z\lambda\right)\right]=e^{-A(\lambda)x+B(\lambda)y}=\overline{v_{\overline\lambda}}.
$$

It also solves the adjoint equation.

## ↑ Ancestors (11)

1. [Ii](../ii.md)
2. [3](../../3.md)
3. [Paper 328](../../../paper-328-split.md)
4. [Iii](../../../split.md)
5. [2016](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
