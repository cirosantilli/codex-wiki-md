<h1 id="b/4/iii/solution">Solution</h1>

↑ **Parent:** [Iii](../iii.md)

Let $g=f^{-1}$, so $g(z)=\sqrt{1-z^{-2}}$, choosing the analytic branch with $\operatorname{Im}g>0$; for example $g(1/2)=i\sqrt3$. Let $\zeta\in\Omega$ be the source point. For the convention $-\Delta G=\delta_\zeta$, the [Dirichlet Green function](../../../../../dirichlet-green-function.md) in the [upper half-plane](../../../../../upper-half-plane-complex-analysis.md) is obtained by an opposite-sign reflected source:

$$
G_H(Z,W)=\frac1{2\pi}\log\left|\frac{Z-\overline W}{Z-W}\right|.
$$

It vanishes for real $Z$, has the [logarithmic singularity](../../../../../logarithmic-singularity.md) $-(2\pi)^{-1}\log|Z-W|$, and is harmonic elsewhere. Conformal invariance of two-dimensional harmonic functions now gives

$$
\boxed{G_\Omega(z,\zeta)=\frac1{2\pi}\log\left|
\frac{g(z)-\overline{g(\zeta)}}{g(z)-g(\zeta)}\right|.}
$$

The branch specified above maps every boundary bank to the real axis, so the Green function vanishes on both slit banks and the vertical wall. Local conformality preserves the coefficient of the [logarithmic singularity](../../../../../logarithmic-singularity.md). If the convention is instead $\Delta G=\delta_\zeta$, negate this expression.

## ↑ Ancestors (13)

1. [Iii](../iii.md)
2. [4](../../4.md)
3. [B](../../../b.md)
4. [2010](../../../../2010-split.md)
5. [Past exam of the perturbation methods and applied complex variables course of the University of Oxford](../../../../split.md)
6. [Perturbation methods and applied complex variables course of the University of Oxford](../../../../../perturbation-methods-and-applied-complex-variables-course-of-the-university-of-oxford.md)
7. [Year 4 of the mathematics course of the University of Oxford](../../../../../year-4-of-the-mathematics-course-of-the-university-of-oxford.md)
8. [Mathematics course of the University of Oxford](../../../../../mathematics-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../split.md)
