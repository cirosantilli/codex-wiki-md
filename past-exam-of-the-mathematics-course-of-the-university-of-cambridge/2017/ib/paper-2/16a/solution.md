<h1 id="16a/solution">Solution</h1>

↑ **Parent:** [16A](../16a.md)

Put $\phi=R(r)\Theta(\theta)Z(z)$ in the [Laplace equation in cylindrical coordinates](../../../../../laplace-equation-in-cylindrical-coordinates.md). [Separation of variables](../../../../../separation-of-variables.md) first gives $\Theta''+m^2\Theta=0$; $2\pi$-periodicity forces $m=0,1,2,\ldots$, with angular factors $\cos m\theta,\sin m\theta$ (only the constant for $m=0$). Taking $Z''=\kappa^2Z$ gives

$$
r^2R''+rR'+(\kappa^2r^2-m^2)R=0.
$$

For $\kappa>0$ the separated modes are therefore

$$
\boxed{[A J_m(\kappa r)+B Y_m(\kappa r)]
[C e^{\kappa z}+D e^{-\kappa z}]
[E\cos m\theta+F\sin m\theta].}
$$

Here $J_m$ and $Y_m$ are the [Bessel function of the first kind](../../../../../bessel-function-of-the-first-kind.md) and the [Bessel function of the second kind](../../../../../bessel-function-of-the-second-kind.md). For the opposite sign $Z''=-\kappa^2 Z$, the modes instead involve $I_m(\kappa r),K_m(\kappa r)$, the [modified Bessel functions](../../../../../modified-bessel-function.md), paired with $\cos\kappa z,\sin\kappa z$. At zero separation constant use $Z=C+Dz$ and $R=Ar^m+Br^{-m}$ for $m\ge1$, or $R=A+B\log r$ for $m=0$. Superpositions over the integer angular orders and appropriate sums or integrals over the separation parameter give the general separated expansion; boundary conditions select its spectrum and coefficients. Regularity at the axis excludes $Y_m,K_m,r^{-m},\log r$ terms.

For the specified decaying side data, bounded separated modes use $e^{-\kappa z}J_m(\kappa r)$. A particular solution is

$$
\boxed{\phi_p=e^{-4z}\left[\frac{J_1(4r)}{J_1(4)}\cos\theta+\frac{J_2(4r)}{J_2(4)}\sin2\theta\right]
+2e^{-z}\frac{J_2(r)}{J_2(1)}\sin2\theta.}
$$

All three denominators are nonzero. Each term satisfies the radial [Bessel differential equation](../../../../../bessel-differential-equation.md), is regular at the axis and bounded for $0\le r\le1,z\ge0$, and substitution at $r=1$ gives the stated side values. The modes behave as $r^m$ at the axis, so their apparent angular dependence there causes no singularity.

There is an actual nonuniqueness in the printed problem: no values are specified at $z=0$. If $j_{0,1}$ is the first positive zero of $J_0$, then for every real $a$,

$$
\phi_p+a e^{-j_{0,1}z}J_0(j_{0,1}r)
$$

is another bounded solution with the same side values. It remains smooth at the axis and even decays as $z\to\infty$. This explicitly proves that [side boundary data do not determine a bounded harmonic function in a half-cylinder](../../../../../side-boundary-data-do-not-determine-a-bounded-harmonic-function-in-a-half-cylinder.md). Thus the boxed expression supplies a bounded solution; the phrase “the bounded solution” is not justified without an additional base boundary condition. The PDF has $z\ge0$, whereas the TeX transcription displays $z>0$.

## ↑ Ancestors (10)

1. [16A](../16a.md)
2. [Paper 2](../../paper-2-split.md)
3. [Ib](../../split.md)
4. [2017](../../../split.md)
5. [Past exam of the mathematics course of the University of Cambridge](../../../../split.md)
6. [Mathematics course of the University of Cambridge](../../../../../mathematics-course-of-the-university-of-cambridge.md)
7. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
8. [University of Cambridge](../../../../../university-of-cambridge-split.md)
9. [List of universities](../../../../../list-of-universities.md)
10. [Codex Wiki](../../../../../split.md)
