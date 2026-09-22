<h1 id="6/c/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**The conventional relaxation-loss peak near $\omega\tau=1$ applies to fixed [strain](../../../../../../strain.md) amplitude, not to fixed [stress](../../../../../../stress.md) amplitude.** This distinction matters because the question explicitly describes oscillating [stress](../../../../../../stress.md).

The full [complex modulus](../../../../../../complex-modulus.md) of the series Maxwell element is

$$
E^*=\frac{ki\omega\tau}{1+i\omega\tau},\qquad
E''=\frac{k\omega\tau}{1+\omega^2\tau^2}.
$$

For imposed [strain](../../../../../../strain.md) $\varepsilon=\varepsilon_0\cos\omega t$, the energy dissipated per volume per cycle is

$$
W_\varepsilon=\pi E''\varepsilon_0^2.
$$

Since $x/(1+x^2)$ has its maximum at $x=1$, **fixed-strain loss per cycle peaks at $\omega^2=\tau^{-2}$**. At that scale the imposed cycle time is comparable with the [relaxation time](../../../../../../relaxation-time.md), and substantial viscous flow occurs while [stress](../../../../../../stress.md) remains appreciable.

For the literally stated comparison with fixed [stress](../../../../../../stress.md) amplitude, use the compliance

$$
J^*=\frac1k+\frac1{i\omega\eta}.
$$

The [dashpot](../../../../../../dashpot.md) [strain](../../../../../../strain.md) rate is $\dot\varepsilon_d=\sigma/\eta$. Its dissipation integrated over a period gives

$$
\boxed{W_\sigma=\int_0^{2\pi/\omega}\frac{\sigma_0^2\cos^2\omega t}{\eta}\,dt
=\frac{\pi\sigma_0^2}{\eta\omega}.}
$$

This decreases monotonically with frequency; **there is no finite-frequency maximum at fixed [stress](../../../../../../stress.md) amplitude in the ideal [Maxwell model](../../../../../../linear-maxwell-fluid.md)**. Its mean dissipated [power](../../../../../../power.md) is $\sigma_0^2/(2\eta)$, independent of frequency. The formal low-frequency divergence in energy per cycle accompanies very large [strain](../../../../../../strain.md) excursions and cannot be extrapolated beyond the linear model's range. The graph identifies both results rather than assigning the fixed-strain peak to the wrong loading condition.

## ↑ Ancestors (14)

1. [Ii](../ii.md)
2. [C](../../c.md)
3. [6](../../../6.md)
4. [Paper 1](../../../../paper-1-split.md)
5. [2018](../../../../split.md)
6. [Past exam of the materials science course of the University of Cambridge](../../../../../split.md)
7. [Materials science course of the University of Cambridge](../../../../../../materials-science-course-of-the-university-of-cambridge.md)
8. [Year 1 of the natural sciences course of the University of Cambridge](../../../../../../year-1-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../../split.md)
