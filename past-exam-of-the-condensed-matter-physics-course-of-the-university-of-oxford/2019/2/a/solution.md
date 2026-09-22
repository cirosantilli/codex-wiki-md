<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The [Einstein model of a solid](../../../../einstein-solid.md) replaces the vibrations of $N$ identical atoms by $3N$ independent [quantum harmonic oscillators](../../../../quantum-harmonic-oscillator-split.md) with a common frequency $\omega_E$. Each atom has three displacement directions; the restoring force is harmonic, coupling between different atoms is replaced by a fixed local restoring potential, and anharmonicity and frequency dispersion are neglected. The crystal volume and $\omega_E$ are held fixed when calculating the vibrational [heat capacity at constant volume](../../../../heat-capacity-at-constant-volume.md).

The one-oscillator [partition function](../../../../canonical-partition-function.md) is

$$
z=\sum_{n=0}^\infty e^{-\beta\hbar\omega_E(n+1/2)}=\frac{e^{-\beta\hbar\omega_E/2}}{1-e^{-\beta\hbar\omega_E}},\qquad Z=z^{3N}.
$$

Consequently, with $T_E=\hbar\omega_E/k_B$,

$$
U=-\frac{\partial\log Z}{\partial\beta}=3N\hbar\omega_E\left[\frac12+\frac1{e^{T_E/T}-1}\right].
$$

Differentiating at fixed volume gives

$$
\boxed{C_V=3Nk_B\left(\frac{T_E}{T}\right)^2\frac{e^{T_E/T}}{(e^{T_E/T}-1)^2}.}
$$

The [zero-point energy](../../../../zero-point-energy.md) does not contribute to this derivative. The result tends to the [Dulong-Petit law](../../../../dulong-petit-law.md) $3Nk_B$ at high temperature and vanishes exponentially at low temperature; the latter is a limitation of the single-frequency model for a real acoustic spectrum.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [2](../../2.md)
3. [2019](../../../2019-split.md)
4. [Past exam of the condensed matter physics course of the University of Oxford](../../../split.md)
5. [Condensed matter physics course of the University of Oxford](../../../../condensed-matter-physics-course-of-the-university-of-oxford.md)
6. [Year 3 of the physics course of the University of Oxford](../../../../year-3-of-the-physics-course-of-the-university-of-oxford.md)
7. [Physics course of the University of Oxford](../../../../physics-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../university-of-oxford-split.md)
11. [List of universities](../../../../list-of-universities.md)
12. [Codex Wiki](../../../../split.md)
