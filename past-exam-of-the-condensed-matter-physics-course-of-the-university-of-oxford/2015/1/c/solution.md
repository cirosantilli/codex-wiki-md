<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

The [Debye model](../../../../debye-model.md) treats the crystal as an isotropic elastic continuum with independent harmonic vibrational modes. There are three acoustic [polarizations](../../../../polarization-waves.md), approximated by linear dispersions and a common effective speed. A cutoff is chosen to retain $3N$ modes for $N$ atoms. The model neglects anharmonic interactions and the detailed high-wavevector dispersion. In a multi-atom primitive cell, optical branches require additional treatment; copper has one atom per primitive cell even though its conventional cubic cell contains four atoms.

A [frequency](../../../../frequency.md) interval contains, per [volume](../../../../volume.md),

$$
g_{\rm ph}(\omega)\,d\omega=3\frac{4\pi q^2dq}{(2\pi)^3}
=\frac{3\omega^2}{2\pi^2c^3}\,d\omega
=\frac{9n\omega^2}{\omega_D^3}\,d\omega.
$$

Each [phonon](../../../../phonon.md) mode has [Bose-Einstein distribution](../../../../bose-einstein-distribution.md) occupation $(e^{\hbar\omega/(k_BT)}-1)^{-1}$. The fixed [zero-point energy](../../../../zero-point-energy.md) contributes no [heat capacity](../../../../heat-capacity.md). Its [thermal energy](../../../../thermal-energy.md) density is

$$
u_{\rm ph}=\frac{9n\hbar}{\omega_D^3}\int_0^{\omega_D}\frac{\omega^3\,d\omega}{e^{\hbar\omega/(k_BT)}-1}
=9nk_BT\left(\frac{T}{\theta_D}\right)^3\int_0^{\theta_D/T}\frac{x^3\,dx}{e^x-1}.
$$

For $T\ll\theta_D$, extending the upper limit to infinity gives $u_{\rm ph}=(3\pi^4/5)nk_BT^4/\theta_D^3$. Therefore

$$
\boxed{C_{\rm ph}=\frac{12\pi^4}{5}nk_B\left(\frac{T}{\theta_D}\right)^3
=\frac{2\pi^2k_B^4}{5\hbar^3c^3}T^3}.
$$

The cubic law reflects the three-dimensional acoustic mode density proportional to $\omega^2$. It is a low-temperature limit, not a valid extrapolation through the classical high-temperature regime.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [1](../../1.md)
3. [2015](../../../2015-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
