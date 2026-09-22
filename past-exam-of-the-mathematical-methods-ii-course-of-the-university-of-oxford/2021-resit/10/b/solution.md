<h1 id="10/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

A reference string segment $dx$ has [mass](../../../../mass.md) $\mu\,dx$ and transverse [velocity](../../../../velocity.md) $y_t$. Its [kinetic energy](../../../../kinetic-energy.md) is $dK=\mu y_t^2\,dx/2$. In the small-slope approximation its extra [arc length](../../../../arc-length.md) is

$$
d\ell-dx=\bigl(\sqrt{1+y_x^2}-1\bigr)dx
=\frac12y_x^2\,dx+O(y_x^4)\,dx.
$$

The [work](../../../../work.md) against constant [tension](../../../../tension.md) $T$ supplies the corresponding [elastic potential energy](../../../../elastic-energy.md) $dU=T(d\ell-dx)$. To quadratic order, the [energy density](../../../../energy-density.md) per unit reference length is therefore

$$
\boxed{u=\frac{d(K+U)}{dx}
=\frac12\left(\mu y_t^2+Ty_x^2\right).}
$$

For the [travelling wave](../../../../travelling-wave.md) $y=A\cos(kx-\omega t+\phi)$, the [wave equation](../../../../wave-equation-split.md) implies $\omega^2=(T/\mu)k^2$. Its [kinetic energy density](../../../../kinetic-energy-density.md) and elastic [energy density](../../../../energy-density.md) are equal, so

$$
u(x,t)=\mu A^2\omega^2\sin^2(kx-\omega t+\phi).
$$

The [energy per wavelength of a transverse string wave](../../../../energy-per-wavelength-of-a-transverse-string-wave.md) comes from integration over any full [wavelength](../../../../wavelength.md) $\lambda=2\pi/|k|$:

$$
\boxed{E_\lambda=\int_{x_*}^{x_*+\lambda}u(x,t)\,dx
=\frac12\mu A^2\omega^2\lambda,\qquad
\langle u\rangle=\frac12\mu A^2\omega^2.}
$$

**The printed expression for energy per wavelength is missing a factor $\lambda$.** Its right-hand side is the mean [energy density](../../../../energy-density.md), with units of [energy](../../../../energy-split.md) per length. For a concrete counterexample within the small-slope regime, take $\mu=1\,\mathrm{kg\,m^{-1}}$, $T=1\,\mathrm N$, $A=0.01\,\mathrm m$ and $\omega=\pi\,\mathrm{s^{-1}}$. Then $\lambda=2\,\mathrm m$ and direct integration gives $E_\lambda=10^{-4}\pi^2\,\mathrm J$, whereas the printed right-hand side is $5\times10^{-5}\pi^2\,\mathrm{J\,m^{-1}}$. It cannot equal an [energy](../../../../energy-split.md).

## ↑ Ancestors (12)

1. [B](../b.md)
2. [10](../../10.md)
3. [2021 resit](../../../2021-resit-split.md)
4. [Past exam of the mathematical methods II course of the University of Oxford](../../../split.md)
5. [Mathematical methods II course of the University of Oxford](../../../../mathematical-methods-ii-course-of-the-university-of-oxford.md)
6. [Year 1 of the physics course of the University of Oxford](../../../../year-1-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
