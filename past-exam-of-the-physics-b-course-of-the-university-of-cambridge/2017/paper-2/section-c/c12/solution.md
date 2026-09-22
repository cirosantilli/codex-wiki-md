<h1 id="section-c/c12/solution">Solution</h1>

↑ **Parent:** [C12](../c12.md)

For a classical dilute [ideal gas](../../../../../ideal-gas-split.md) in [thermal equilibrium](../../../../../thermal-equilibrium-split.md), the [probability](../../../../../probability.md) of a single-particle [velocity](../../../../../velocity.md) is proportional to the [Boltzmann factor](../../../../../boltzmann-factor.md) for [kinetic energy](../../../../../kinetic-energy.md), $e^{-mv^2/(2k_BT)}$. [Velocities](../../../../../velocity.md) with [speed](../../../../../speed.md) between $v$ and $v+dv$ fill a spherical shell of velocity-space [volume](../../../../../volume-thermodynamics.md) $4\pi v^2dv$. The normalized [Maxwell speed distribution](../../../../../maxwell-speed-distribution.md) is therefore

$$
f(v)=4\pi\left(\frac{m}{2\pi k_BT}\right)^{3/2}v^2e^{-mv^2/(2k_BT)},\qquad v\geq0.
$$

The factor $v^2$ counts states, rather than representing an extra Boltzmann [energy](../../../../../energy-split.md) factor.

Set $\alpha=m/(2k_BT)$ and use $I_j=\int_0^\infty v^j e^{-\alpha v^2}dv$. Normalization cancels in ratios, so the given recurrence gives

$$
\overline v=\frac{I_3}{I_2}=\frac{2}{\sqrt{\pi\alpha}}
=\sqrt{\frac{8k_BT}{\pi m}},\qquad
\overline{v^2}=\frac{I_4}{I_2}=\frac{3}{2\alpha}=\frac{3k_BT}{m}.
$$

Consequently

$$
\boxed{\overline{v^2}=\frac{3\pi}{8}\,\overline v^{\,2}.}
$$

The [root mean square](../../../../../root-mean-square.md) [speed](../../../../../speed.md) is larger than the [mean](../../../../../expected-value-split.md) [speed](../../../../../speed.md), consistent with the positive [variance](../../../../../variance-split.md) of the [speed distribution](../../../../../speed-distribution.md).

## ↑ Ancestors (14)

1. [C12](../c12.md)
2. [Section C](../../section-c.md)
3. [Paper 2](../../../paper-2-split.md)
4. [2017](../../../split.md)
5. [Past exam of the physics B course of the University of Cambridge](../../../../split.md)
6. [Physics B course of the University of Cambridge](../../../../../physics-b-course-of-the-university-of-cambridge.md)
7. [Physics course of the year 2 of the natural sciences course of the University of Cambridge](../../../../../physics-course-of-the-year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
8. [Year 2 of the natural sciences course of the University of Cambridge](../../../../../year-2-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
9. [Year of the natural sciences course of the University of Cambridge](../../../../../year-of-the-natural-sciences-course-of-the-university-of-cambridge.md)
10. [Natural sciences course of the University of Cambridge](../../../../../natural-sciences-course-of-the-university-of-cambridge.md)
11. [Course of the University of Cambridge](../../../../../course-of-the-university-of-cambridge.md)
12. [University of Cambridge](../../../../../university-of-cambridge-split.md)
13. [List of universities](../../../../../list-of-universities.md)
14. [Codex Wiki](../../../../../split.md)
