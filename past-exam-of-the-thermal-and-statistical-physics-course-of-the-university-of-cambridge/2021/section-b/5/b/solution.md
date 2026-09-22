<h1 id="section-b/5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

For $N$ indistinguishable classical [particles](../../../../../particle-physics.md) the [canonical partition function](../../../../../canonical-partition-function.md) is an [integral](../../../../../integral-split.md) over [phase space](../../../../../phase-space.md),

$$
Z_N=\frac{1}{N!h^{3N}}\int_{V^N}\prod_{i=1}^N d^3r_i\int\prod_{i=1}^Nd^3p_i\,
\exp\left[-\beta\sum_i\frac{p_i^2}{2m}-\frac\beta2\sum_{i\ne j}\phi(r_{ij})\right].
$$

The factor $1/N!$ removes overcounting under [particle](../../../../../particle-physics.md) permutations, and $h^{3N}$ makes the classical phase-space measure dimensionless. The [pair potential](../../../../../pair-potential.md) depends only on positions, so all momentum integrations separate. The three-dimensional [Gaussian integral](../../../../../gaussian-integral.md) for each [particle](../../../../../particle-physics.md) gives

$$
\frac1{h^3}\int_{\mathbb R^3}e^{-\beta p^2/(2m)}d^3p
=\frac1{h^3}\left(\frac{2\pi m}{\beta}\right)^{3/2}
=\lambda^{-3},\qquad
\lambda=\sqrt{\frac{2\pi\hbar^2\beta}{m}}.
$$

The [grand canonical partition function](../../../../../grand-canonical-partition-function.md) is $\Xi=\sum_{N=0}^\infty e^{\beta\mu N}Z_N$, where [chemical potential](../../../../../chemical-potential-split.md) $\mu$ controls the mean number of [particles](../../../../../particle-physics.md). Therefore

$$
\boxed{\Xi=\sum_{N=0}^\infty\frac1{N!}\left(\frac{e^{\beta\mu}}{\lambda^3}\right)^N
\int_{V^N}\prod_{i=1}^Nd^3r_i\,
\exp\left[-\frac\beta2\sum_{i\ne j}\phi(r_{ij})\right].}
$$

For $N=0$, the empty products and configurational [integral](../../../../../integral-split.md) equal one. The factor $1/2$ in the interaction prevents double counting of unordered [particle](../../../../../particle-physics.md) pairs.

## ↑ Ancestors (14)

1. [B](../b.md)
2. [5](../../5.md)
3. [Section B](../../../section-b.md)
4. [2021](../../../../2021-split.md)
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
