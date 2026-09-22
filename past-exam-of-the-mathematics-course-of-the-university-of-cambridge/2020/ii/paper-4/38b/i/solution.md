<h1 id="38b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

Let the disturbed sheet be $y=h+\eta$ and take a [normal mode](../../../../../../normal-mode.md) proportional to $e^{i(kx-\omega t)}$, with $K=|k|$. [Irrotational flow](../../../../../../irrotational-flow.md) and the rigid-wall condition at $y=0$ give perturbation [velocity potentials](../../../../../../velocity-potential.md)

$$
\phi_-'=A\cosh(Ky)e^{i(kx-\omega t)},
\qquad
\phi_+'=Be^{-K(y-h)}e^{i(kx-\omega t)}.
$$

The two linearized [kinematic boundary conditions](../../../../../../kinematic-boundary-condition.md) at $y=h$ are

$$
-i(\omega-kU)\eta=AK\sinh(Kh),
\qquad
-i\omega\eta=-KB.
$$

The [Unsteady Bernoulli equation](../../../../../../unsteady-bernoulli-equation.md) gives $p_-'=i\rho(\omega-kU)A\cosh(Kh)$ and $p_+'=i\rho\omega B$. Continuity of pressure therefore yields the [finite-depth vortex-sheet dispersion relation](../../../../../../finite-depth-vortex-sheet-dispersion-relation.md)

$$
\boxed{(\omega-kU)^2\coth(Kh)+\omega^2=0},
$$

or, with $T=\tanh(Kh)$,

$$
(\omega-kU)^2+T\omega^2=0.
$$

For $k>0$ its two roots are

$$
\boxed{\omega=\frac{kU}{1+T}\left(1\pm i\sqrt T\right)}.
$$

One root has positive temporal growth for every $k\ne0$, so every finite [wavelength](../../../../../../wavelength.md) is subject to the [Kelvin-Helmholtz instability](../../../../../../kelvin-helmholtz-instability.md).

## ↑ Ancestors (11)

1. [I](../i.md)
2. [38B](../../38b.md)
3. [Paper 4](../../../paper-4-split.md)
4. [Ii](../../../split.md)
5. [2020](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
