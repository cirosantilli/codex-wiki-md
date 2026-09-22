<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The isothermal volume [compressibility](../../../../isothermal-compressibility.md) is $\kappa=-(1/V)(\partial V/\partial p)_T$. For isotropic cubic compression $V\propto a^3$ and $d_{hkl}=a/\sqrt{h^2+k^2+l^2}$, so

$$
\frac1{d_{hkl}}\left(\frac{\partial d_{hkl}}{\partial p}\right)_T
=\frac1a\left(\frac{\partial a}{\partial p}\right)_T=-\frac\kappa3.
$$

[Differentiate](../../../../derivative.md) [Bragg's law](../../../../bragg-s-law.md) $2d_{hkl}\sin\theta=\lambda$ at fixed incident [wavelength](../../../../wavelength.md) and fixed reflection:

$$
0=\sin\theta\frac{\partial d}{\partial p}+d\cos\theta\frac{\partial\theta}{\partial p},
\qquad\boxed{\left(\frac{\partial\theta}{\partial p}\right)_T=\frac\kappa3\tan\theta,\quad\alpha=\frac13.}
$$

This [derivative](../../../../derivative.md) uses radians. It remains locally valid with a pressure-dependent [compressibility](../../../../isothermal-compressibility.md), provided the cubic isotropic phase is retained. For a constant stipulated $\kappa$, integration gives

$$
\boxed{a(p)=a_0e^{-\kappa p/3},\qquad
\sin\theta(p)=\sin\theta_0e^{\kappa p/3}.}
$$

Thus $a_0(1-\kappa p/3)$ is only the first-order approximation, not the exact consequence of a constant logarithmic [compressibility](../../../../isothermal-compressibility.md). The finite-pressure calculation also assumes that the reflection still exists, the [crystal](../../../../crystal.md) remains in the same structure and $\sin\theta_0e^{\kappa p/3}\leq1$. These limitations matter for a large extrapolation.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2016](../../../2016-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
