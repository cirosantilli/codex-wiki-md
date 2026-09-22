<h1 id="2/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The harmonic [phonon](../../../../phonon.md) contribution to the [internal energy](../../../../internal-energy-split.md) is

$$
U=\int_0^{\omega_D}g(\omega)\hbar\omega
\left[\frac12+\frac1{e^{\hbar\omega/(k_BT)}-1}\right]d\omega.
$$

For $T\gg\Theta_D$, every retained mode has $x=\hbar\omega/(k_BT)\ll1$. Expanding $1/(e^x-1)=1/x-1/2+O(x)$ cancels the explicit half quantum and gives $k_BT$ per mode to leading order. Therefore

$$
U=3Nk_BT+O\!\left(\frac{N(k_B\Theta_D)^2}{k_BT}\right),
\qquad\boxed{C_V=\left(\frac{\partial U}{\partial T}\right)_V\longrightarrow3Nk_B.}
$$

Equivalently, differentiating before integrating gives

$$
C_V=9Nk_B\left(\frac{T}{\Theta_D}\right)^3\int_0^{\Theta_D/T}\frac{x^4e^x}{(e^x-1)^2}\,dx.
$$

The integrand tends to $x^2$, and its integral is $(\Theta_D/T)^3/3$, producing the same [Dulong-Petit law](../../../../dulong-petit-law.md). In classical language, the [equipartition theorem](../../../../equipartition-theorem.md) assigns $k_BT/2$ each to the kinetic and elastic parts of every harmonic [normal mode](../../../../normal-mode.md). Fixed [zero-point energy](../../../../zero-point-energy.md) does not contribute to the [heat capacity](../../../../heat-capacity.md).

## ↑ Ancestors (12)

1. [C](../c.md)
2. [2](../../2.md)
3. [2012](../../../2012-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
