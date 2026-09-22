<h1 id="section-a/a1/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

Particles within each species are indistinguishable, while the two species are physically distinguishable and their numbers are fixed. Independence makes the [canonical partition function](../../../../../canonical-partition-function.md) factor by species:

$$
\boxed{Z=\frac{Z_1^{N_A}}{N_A!}\frac{Z_1^{N_B}}{N_B!}
=\frac{Z_1^N}{N_A!N_B!},\qquad N=N_A+N_B.}
$$

Since $Z_1\propto T^{3/2}$ at fixed [volume](../../../../../volume-thermodynamics.md), $U=-\partial_\beta\ln Z=3Nk_BT/2$. The canonical [entropy](../../../../../entropy-split.md) is therefore

$$
\boxed{S=k_B\left[N\ln Z_1-\ln(N_A!)-\ln(N_B!)+\frac32N\right].}
$$

For large species populations, [Stirling's approximation](../../../../../stirling-formula.md) gives the equivalent [Sackur-Tetrode equation](../../../../../sackur-tetrode-equation.md) form

$$
\boxed{S\simeq k_B\sum_{i=A,B}N_i\left[\ln\frac{Z_1}{N_i}+\frac52\right].}
$$

For structureless particles with the same translational [partition function](../../../../../canonical-partition-function.md), $Z_1=V/\lambda^3$, where $\lambda$ is their common [thermal de Broglie wavelength](../../../../../thermal-de-broglie-wavelength.md). More generally the supplied common constant factor in $Z_1$ should be retained in the [entropy](../../../../../entropy-split.md).

Writing $x_i=N_i/N$ separates the total-number contribution from the composition term:

$$
S\simeq Nk_B\left[\ln\frac{Z_1}{N}+\frac52\right]
-Nk_B(x_A\ln x_A+x_B\ln x_B).
$$

The last term is the [entropy of mixing](../../../../../entropy-of-mixing.md) relative to separated ideal components at the same [temperature](../../../../../temperature-split.md) and [pressure](../../../../../pressure-split.md). This is the [entropy of a two-species classical ideal gas](../../../../../entropy-of-a-two-species-classical-ideal-gas.md). Artificially labeling otherwise identical [chemical atoms](../../../../../atom-physics.md) would not justify dividing by separate factorials or adding a mixing [entropy](../../../../../entropy-split.md). The pure-species [limit](../../../../../limit-of-a-function.md) is obtained by $x\ln x\to0$.

## ↑ Ancestors (14)

1. [C](../c.md)
2. [A1](../../a1.md)
3. [Section A](../../../section-a.md)
4. [2018](../../../../2018-split.md)
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
