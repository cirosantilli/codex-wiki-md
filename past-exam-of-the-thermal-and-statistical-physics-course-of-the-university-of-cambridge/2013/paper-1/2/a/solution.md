<h1 id="2/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

[Equipartition](../../../../../equipartition-theorem.md) gives mean [energy](../../../../../energy-split.md) $k_BT/2$ for each [independent](../../../../../independent-random-variables.md) quadratic term in a classical canonical [Hamiltonian](../../../../../hamiltonian.md). For example, $p^2/(2m)$ and $kx^2/2$ each contribute this amount in a [harmonic oscillator](../../../../../simple-harmonic-motion.md). It is a thermal average, not an instantaneous equality; constraints, nonquadratic terms or quantum level spacings large compared with $k_BT$ require a different calculation.

The [fluctuation-dissipation theorem](../../../../../fluctuation-dissipation-theorem.md) connects equilibrium fluctuations with the dissipative part of [linear response](../../../../../linear-response-theory.md). If an applied [force](../../../../../force-split.md) couples as $-f(t)x$, use response to $e^{-i\omega t}$ and define the two-sided angular-frequency spectrum $S_{xx}(\omega)=\int e^{i\omega t}\langle\delta x(t)\delta x(0)\rangle dt$. The classical relation is

$$
\boxed{S_{xx}(\omega)=\frac{2k_BT}{\omega}\operatorname{Im}\chi(\omega).}
$$

For a viscously damped particle, $m\dot v=-\zeta v+\xi(t)$, the corresponding white-noise [force](../../../../../force-split.md) satisfies $\langle\xi(t)\xi(t')\rangle=2\zeta k_BT\delta(t-t')$. Noise replenishes [energy](../../../../../energy-split.md) lost by [friction](../../../../../friction.md); their strengths cannot be varied independently at fixed equilibrium [temperature](../../../../../temperature-split.md).

Electrically, the one-sided voltage-noise spectrum per hertz of an equilibrium [resistor](../../../../../resistor.md) is $4k_BTR$. A [capacitor](../../../../../capacitor.md) in parallel filters it to

$$
S_V^{(1)}(f)=\frac{4k_BTR}{1+(2\pi fRC)^2},\qquad
\int_0^\infty S_V^{(1)}(f)\,df=\frac{k_BT}{C}.
$$

The same equilibrium [voltage](../../../../../voltage.md) [variance](../../../../../variance-split.md) follows from [equipartition](../../../../../equipartition-theorem.md). Increasing R makes the spectrum taller and narrower without changing its integrated area. This thermodynamic connection between dissipative conductance and thermal electrical fluctuations is the content of the classical noise calculation.[1928, abstract: equilibrium thermodynamic and statistical calculation of thermal electromotive force](../../../../../thermal-agitation-of-electric-charge-in-conductors-by-harry-nyquist.md)

<a id="2/a/image-original-normalized-resistor-capacitor-noise-spectra-increasing-resistance-changes-the-spectral-width-and-height-while-preserving-the-full-equilibrium-variance"></a>
![](../../../../../past-exam-of-the-thermal-and-statistical-physics-course-of-the-university-of-cambridge/2013/paper-1-tsp2013-equilibrium-noise.png)

**[Figure 2](#2/a/image-original-normalized-resistor-capacitor-noise-spectra-increasing-resistance-changes-the-spectral-width-and-height-while-preserving-the-full-equilibrium-variance). Original normalized resistor-capacitor noise spectra: increasing resistance changes the spectral width and height while preserving the full equilibrium variance**.

## ↑ Ancestors (14)

1. [A](../a.md)
2. [2](../../2.md)
3. [Paper 1](../../../paper-1-split.md)
4. [2013](../../../split.md)
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
