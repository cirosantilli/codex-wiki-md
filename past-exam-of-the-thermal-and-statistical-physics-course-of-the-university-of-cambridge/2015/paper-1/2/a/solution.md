<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

A non-ideal gas departs from $p=nk_BT$ because interactions and finite particle size affect its [pressure](../../../../../pressure-split.md). At sufficiently low [number density](../../../../../number-density.md) $n=N/V$, the [virial expansion](../../../../../virial-expansion.md) separates these corrections:

$$
\boxed{\frac{p}{nk_BT}=1+B_2(T)n+B_3(T)n^2+\cdots}.
$$

The [second virial coefficient](../../../../../second-virial-coefficient.md) has dimensions of [volume](../../../../../volume.md) per particle, while $B_3$ has dimensions of [volume](../../../../../volume.md) squared. These are density-series coefficients, not the coefficients of a pressure-series expansion with the same names.

For classical particles interacting through a [pair potential](../../../../../pair-potential.md) $u(r)$,

$$
B_2(T)=2\pi\int_0^\infty[1-e^{-u(r)/(k_BT)}]r^2\,dr.
$$

Repulsion contributes positively and attraction negatively. A hard core of diameter $d$ gives $B_2=2\pi d^3/3$, four times the geometric [volume](../../../../../volume.md) of one sphere. The factor reflects the [volume](../../../../../volume.md) excluded to the centre of a second particle together with pair counting; it is not simply the occupied geometric [volume](../../../../../volume.md).

Expanding the [Van der Waals equation](../../../../../van-der-waals-equation.md) at $nb\ll1$ gives

$$
\frac p{nk_BT}=\frac1{1-nb}-\frac{an}{k_BT}
=1+\left(b-\frac a{k_BT}\right)n+b^2n^2+\cdots.
$$

The [virial coefficients of the van der Waals gas](../../../../../virial-coefficients-of-the-van-der-waals-gas.md) are therefore $B_2=b-a/(k_BT)$ and $B_3=b^2$. The [Boyle temperature](../../../../../boyle-temperature.md), $T_B=a/(k_Bb)$, makes the leading correction vanish, but does not remove the higher coefficients or turn the gas exactly ideal. More realistic potentials give temperature-dependent higher coefficients that need not equal the van der Waals values.

A useful measurement is a sequence of dilute isothermal [pressure](../../../../../pressure-split.md)–[volume](../../../../../volume.md) observations. Plotting $[p/(nk_BT)-1]/n$ against $n$ exposes $B_2$ as the zero-density intercept and $B_3$ as its initial slope. Control [temperature](../../../../../temperature-split.md) and density calibration, check equilibration and [adsorption](../../../../../adsorption.md) on the container walls, and vary the fitted density interval to test truncation error. One measured virial coefficient cannot uniquely reconstruct the [pair potential](../../../../../pair-potential.md). Near coexistence or a [critical point](../../../../../critical-point.md) a short density series may fail, and at quantum-degenerate densities exchange statistics add corrections even without interactions.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2015](../../../split.md)
5. [Past exam of the thermal and statistical physics course of the University of Cambridge](../../../../split.md)
6. [Thermal and Statistical Physics course of the University of Cambridge](../../../../../thermal-and-statistical-physics-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 3 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 3 of the natural sciences course of the University of Cambridge](../../../../../year-3-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
