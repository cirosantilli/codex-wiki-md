<h1 id="1/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

Let $d=\Delta x$, impose $u_0=u_{M+1}=0$, and write the [method of lines](../../../../../../method-of-lines.md) system as $U'=LU$, where

$$
L=D_2+\kappa D_1,\qquad
D_2=d^{-2}\operatorname{tridiag}(1,-2,1),\quad
(D_1)_{m,m+1}=\frac1{2d},\quad(D_1)_{m+1,m}=-\frac1{2d}.
$$

Thus $D_2$ is a negative definite [symmetric matrix](../../../../../../symmetric-matrix.md) and $D_1$ is a [skew-symmetric matrix](../../../../../../skew-symmetric-matrix.md). Use the mesh-weighted [Euclidean norm](../../../../../../euclidean-norm.md) $\|U\|_d^2=d\sum_{m=1}^M|u_m|^2$. Discrete [summation by parts](../../../../../../abel-s-summation-formula.md) yields the [centered Dirichlet drift-diffusion energy identity](../../../../../../centered-dirichlet-drift-diffusion-energy-identity.md)

$$
\frac12\frac d{dt}\|U\|_d^2
=d\operatorname{Re}(U^*LU)
=-\frac1d\sum_{m=0}^{M}|u_{m+1}-u_m|^2\leq0.
$$

Consequently

$$
\boxed{\|e^{tL}U^0\|_d\leq\|U^0\|_d,\qquad t\geq0.}
$$

The same estimate controls perturbations and is uniform in the number of grid points and in the fixed drift coefficient. Finite-dimensional linear ODE theory guarantees existence, so this proves [stability of a numerical method](../../../../../../stability-of-a-numerical-method.md) for the semidiscretization.

The factor $d^{1/2}$ simply rescales the vector norm and does not change the induced [matrix](../../../../../../matrix.md) norm. Equivalently the symmetric part is $(L+L^*)/2=D_2$, whose largest [eigenvalue](../../../../../../eigenvalue.md) is $-4d^{-2}\sin^2[\pi/(2(M+1))]<0$. This is the [Euclidean logarithmic norm](../../../../../../euclidean-logarithmic-norm.md), rather than generally the [spectral abscissa](../../../../../../spectral-abscissa.md) of a nonnormal [matrix](../../../../../../matrix.md). No periodic [Fourier mode](../../../../../../fourier-mode.md) assumption has been made: the zero endpoint terms are part of the proof. In particular positivity of both off-diagonal coefficients is not needed for this $L^2$ stability result.

## ↑ Ancestors (11)

1. [B](../b.md)
2. [1](../../1.md)
3. [Paper 66](../../../paper-66-split.md)
4. [Iii](../../../split.md)
5. [2014](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
