<h1 id="section-b/6/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

Let $u_r$ be a nonzero admissible mode, multiply the equation of part (d) by its complex conjugate and integrate between the cylinders. The endpoint conditions remove the boundary term in [integration by parts](../../../../../integration-by-parts.md), giving the [Rayleigh stability integral identity](../../../../../rayleigh-stability-integral-identity.md)

$$
\int|u_r'|^2\,dr+\frac{k^2}{\omega^2}\int\Phi|u_r|^2\,dr
=-k^2\int|u_r|^2\,dr.
$$

Rearrange to obtain a real [Rayleigh quotient](../../../../../rayleigh-quotient.md):

$$
\boxed{\omega^2=-\frac{k^2\int\Phi(r)|u_r|^2\,dr}
{\int|u_r'|^2\,dr+k^2\int|u_r|^2\,dr}.}
$$

The denominator is strictly positive. Consequently, with the paper's convention,

$$
\boxed{\Phi(r)<0\ \text{throughout the gap guarantees oscillatory normal-mode stability}.}
$$

The weak inequality $\Phi\le0$ excludes exponentially growing axisymmetric modes, but permits marginal cases and possible algebraic growth when the restoring effect vanishes. Strict negativity avoids that degeneracy. Equivalently, the conventional [Rayleigh discriminant](../../../../../rayleigh-discriminant.md) is positive, or the squared [specific angular momentum](../../../../../specific-angular-momentum.md) increases outward:

$$
\boxed{\frac d{dr}(r^2\Omega)^2>0.}
$$

This is the [Rayleigh centrifugal stability criterion](../../../../../rayleigh-centrifugal-stability-criterion.md). In the suggested [time-independent Schrödinger equation](../../../../../time-independent-schrodinger-equation.md) analogy, a growing mode has $\omega^2<0$; if $\Phi\le0$, its effective potential $k^2\Phi/\omega^2$ is nonnegative. The nonnegative kinetic term and that potential cannot have the required negative eigenvalue $-k^2$, which gives the same exclusion.

As a sign check, for [solid-body rotation](../../../../../solid-body-rotation.md) $\kappa_{\rm ep}^2=4\Omega^2$ and $\Phi=-4\Omega^2$. In a gap of width $d=R_>-R_<$, the radial modes $u_r\propto\sin[n\pi(r-R_<)/d]$ have

$$
\omega_n^2=\frac{4\Omega^2k^2}{k^2+(n\pi/d)^2}>0,
$$

as expected for [inertial waves](../../../../../inertial-wave.md). The argument establishes axisymmetric inviscid stability within the stated thin-gap model, rather than a claim about all perturbations of a viscous flow.

## ↑ Ancestors (14)

1. [E](../e.md)
2. [6](../../6.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
5. [Past exam of the astrophysical fluid dynamics course of the University of Cambridge](../../../../split.md)
6. [Astrophysical Fluid Dynamics course of the University of Cambridge](../../../../../astrophysical-fluid-dynamics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
