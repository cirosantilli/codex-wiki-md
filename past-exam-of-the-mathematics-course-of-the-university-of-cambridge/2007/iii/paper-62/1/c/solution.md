<h1 id="1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

A radial light ray in the [FLRW metric](../../../../../../friedmann-lemaitre-robertson-walker-metric.md) travels [comoving radial distance](../../../../../../comoving-radial-distance.md) $d\chi=dt/a$ in units $c=1$. The [total comoving visibility radius](../../../../../../total-comoving-visibility-radius.md) is therefore the full available [conformal time](../../../../../../conformal-time.md) interval,

$$
d_c=\int_0^\infty\frac{dt}{a(t)}=\int_0^\infty\frac{da}{a^2H(a)}.
$$

Insert the [Friedmann equation](../../../../../../friedmann-equations.md) from part (a), then put $y=1/a$ to get

$$
\boxed{d_c=\frac1{H_0}\int_0^\infty\frac{dy}{\sqrt{1-\Omega_M+\Omega_My^3}}.}
$$

For $0<\Omega_M<1$ the integrand is bounded at zero and decays as $y^{-3/2}$ at infinity, so the [total conformal lifetime of a flat matter-Lambda universe](../../../../../../total-conformal-lifetime-of-a-flat-matter-lambda-universe.md) is finite. Equivalently, this distance is the present [comoving particle horizon](../../../../../../comoving-particle-horizon.md) plus the remaining comoving distance to the [cosmological event horizon](../../../../../../cosmological-event-horizon.md). This describes causal visibility under the assumed ability to see back to the initial singularity.

The substitution $u=y[\Omega_M/(1-\Omega_M)]^{1/3}$ also evaluates the integral using the [beta function](../../../../../../beta-function.md):

$$
d_c=\frac{\Omega_M^{-1/3}(1-\Omega_M)^{-1/6}}{3H_0}\,\mathrm B\!\left(\frac13,\frac16\right).
$$

## ↑ Ancestors (11)

1. [C](../c.md)
2. [1](../../1.md)
3. [Paper 62](../../../paper-62-split.md)
4. [Iii](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
